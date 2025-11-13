# HappyVeneer: Free Website Hosting & Namecheap Domain Setup Guide

**Author:** Manus AI  
**Date:** November 12, 2025  
**Purpose:** This guide provides step-by-step instructions for hosting your "Coming Soon" website for free using GitHub Pages and connecting your custom domain (e.g., `happyveneer.de`) purchased from Namecheap.

---

## 🎯 OVERVIEW

This guide will walk you through a simple, free, and professional way to get your "Coming Soon" page online. We will use:

- **GitHub Pages:** For free, reliable, and fast static website hosting.
- **Namecheap:** To manage your domain's DNS settings and point it to GitHub Pages.

**The entire process takes about 15-20 minutes, plus up to 48 hours for DNS changes to propagate globally.**

---

## 🚀 STEP 1: CREATE A GITHUB REPOSITORY

First, you need a free GitHub account. If you don't have one, sign up at [github.com](https://github.com).

1.  **Create a New Repository:**
    -   Click the **"+"** icon in the top-right corner and select **"New repository"**.
    -   **Repository name:** Must be `your-github-username.github.io` (replace `your-github-username` with your actual GitHub username). This is a special repository that automatically creates a GitHub Pages site.
    -   **Description:** (Optional) "HappyVeneer Coming Soon Page"
    -   **Public/Private:** Select **Public** (required for free GitHub Pages).
    -   Click **"Create repository"**.

---

## 📂 STEP 2: UPLOAD YOUR WEBSITE FILES

Now, we'll upload the `index.html`, `style.css`, and `logo.png` files to your new repository.

1.  **Go to Your Repository:**
    -   Navigate to the `your-github-username.github.io` repository you just created.

2.  **Upload Files:**
    -   Click the **"Add file"** button and select **"Upload files"**.
    -   Drag and drop the `index.html`, `style.css`, and `logo.png` files from your computer into the upload area.
    -   **Commit changes:**
        -   In the "Commit changes" box, type a message like "Initial commit: Add website files".
        -   Click the **"Commit changes"** button.

3.  **Verify Your Site:**
    -   Your website should now be live at `https://your-github-username.github.io`.
    -   Visit this URL in your browser to see your "Coming Soon" page.

---

## 🌐 STEP 3: CONFIGURE YOUR NAMECHEAP DOMAIN

Next, we'll tell Namecheap to point your custom domain (e.g., `happyveneer.de`) to your new GitHub Pages site.

1.  **Log in to Namecheap:**
    -   Go to [namecheap.com](https://www.namecheap.com) and log in to your account.

2.  **Go to Domain List:**
    -   From your Dashboard, click on **"Domain List"** in the left sidebar.

3.  **Manage Your Domain:**
    -   Find your domain (e.g., `happyveneer.de`) and click the **"Manage"** button next to it.

4.  **Advanced DNS Settings:**
    -   Click on the **"Advanced DNS"** tab.

5.  **Add DNS Records for GitHub Pages:**
    -   You will need to add **four `A` records** and **one `CNAME` record**.
    -   **Delete any existing `A` or `CNAME` records** before adding new ones.

    **Add the following four `A` records:**

| Type | Host | Value | TTL |
| :--- | :--- | :--- | :--- |
| `A` Record | `@` | `185.199.108.153` | Automatic |
| `A` Record | `@` | `185.199.109.153` | Automatic |
| `A` Record | `@` | `185.199.110.153` | Automatic |
| `A` Record | `@` | `185.199.111.153` | Automatic |

    **Add the following `CNAME` record:**

| Type | Host | Value | TTL |
| :--- | :--- | :--- | :--- |
| `CNAME` Record | `www` | `your-github-username.github.io` | Automatic |

    *Replace `your-github-username.github.io` with your actual GitHub Pages URL.*

6.  **Save Changes:**
    -   Click the green **"Save All Changes"** checkmark icon for each record you add.

---

## 🔗 STEP 4: LINK YOUR CUSTOM DOMAIN IN GITHUB

Finally, we need to tell GitHub to expect traffic from your custom domain.

1.  **Go to Your Repository Settings:**
    -   Navigate back to your `your-github-username.github.io` repository on GitHub.
    -   Click the **"Settings"** tab.

2.  **Go to Pages Settings:**
    -   In the left sidebar, click on **"Pages"**.

3.  **Add Your Custom Domain:**
    -   Under the **"Custom domain"** section, type your domain name (e.g., `www.happyveneer.de`) in the text box.
    -   Click the **"Save"** button.

4.  **Enforce HTTPS:**
    -   After a few minutes, the page will refresh, and you should see a message saying "Your site is published at `https://www.happyveneer.de`".
    -   Check the box for **"Enforce HTTPS"**. This ensures your site is secure and uses `https://`.

---

## 🎉 COMPLETE!

**That's it!** Your website is now configured.

-   **DNS Propagation:** It can take anywhere from **30 minutes to 48 hours** for the DNS changes to take effect globally. Be patient.
-   **Check Your Site:** Once the DNS has propagated, you will be able to visit `https://www.happyveneer.de` and see your animated "Coming Soon" page.

### **Troubleshooting:**

-   **Site not working after 48 hours?** Double-check the `A` and `CNAME` records in Namecheap. Make sure there are no typos.
-   **GitHub Pages error?** Ensure your repository is public and the custom domain is spelled correctly in the GitHub settings.
-   **Clear your browser cache** if you are still seeing an old version of the site.

---

## 📦 WEBSITE FILES

All necessary files (`index.html`, `style.css`, `logo.png`) are included with this guide. You can find them in the `happyveneer_website` directory.

**Good luck with your launch!**
