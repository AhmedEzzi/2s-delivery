# How to host the privacy policy on GitHub (GitHub Pages)

Google Play requires a **public URL** for your privacy policy. You can host the file `docs/privacy-policy.html` on GitHub Pages for free.

---

## Step 1: Edit the policy (optional)

1. Open **`docs/privacy-policy.html`** in this repo.
2. Set the **"Last updated"** date and add your contact/company details at the end if you want.
3. Commit and push to GitHub.

---

## Step 2: Enable GitHub Pages

1. On **GitHub**, open your repository (e.g. `two_s_delivery-main`).
2. Go to **Settings** (tab at the top of the repo).
3. In the left sidebar, click **Pages** (under "Code and automation" or "Build and deployment").
4. Under **Build and deployment**:
   - **Source**: choose **Deploy from a branch**.
   - **Branch**: select `main` (or your default branch).
   - **Folder**: select **`/ (root)`** or **`/docs`**.
     - If you choose **`/docs`**, GitHub will serve everything inside the `docs` folder. The file `docs/privacy-policy.html` will be at:  
       `https://<your-username>.github.io/<repo-name>/privacy-policy.html`
     - If you choose **`/ (root)`**, you would need to put `privacy-policy.html` in the **root** of the repo for the same URL to work (or use `index.html` for the main page).
5. Click **Save**.
6. Wait 1–2 minutes. GitHub will build and publish the site. The URL will be shown at the top (e.g. `https://username.github.io/repo-name/`).

---

## Step 3: Get your privacy policy URL

- If you use **Folder: /docs** and the file is `docs/privacy-policy.html`:

  **`https://<your-username>.github.io/<repo-name>/privacy-policy.html`**

- Replace:
  - **`<your-username>`** → your GitHub username (e.g. `ahmedezz`)
  - **`<repo-name>`** → the repository name (e.g. `two_s_delivery-main`)

Example: if your username is `ahmedezz` and the repo is `two_s_delivery-main`, the URL is:

**`https://ahmedezz.github.io/two_s_delivery-main/privacy-policy.html`**

- If the repo is under an **organisation**, use the org name:  
  **`https://<org-name>.github.io/<repo-name>/privacy-policy.html`**

---

## Step 4: Use the URL in Google Play Console

1. Open [Google Play Console](https://play.google.com/console) → your app.
2. Go to **Grow** → **Store presence** → **Main store listing**.
3. Find the **Privacy policy** field.
4. Paste the full URL (e.g. `https://ahmedezz.github.io/two_s_delivery-main/privacy-policy.html`).
5. Save.

After that, your release will satisfy the "privacy policy required" requirement for permissions like CAMERA and location.
