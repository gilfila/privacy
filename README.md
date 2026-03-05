# T1D Notifier — Privacy Policy Page

A static privacy policy page for the T1D Notifier app, served at `/privacy`.

## Deploying to Render

### 1. Push this repo to GitHub

Make sure `index.html` is committed and pushed to your GitHub repository.

### 2. Create a new Static Site on Render

1. Go to [render.com](https://render.com) and sign in.
2. Click **New +** → **Static Site**.
3. Connect your GitHub account and select this repository.

### 3. Configure the static site

| Setting | Value |
|---|---|
| **Name** | `t1d-notifier-privacy` (or any name you like) |
| **Branch** | `master` (or `main`) |
| **Root Directory** | *(leave blank)* |
| **Build Command** | *(leave blank — no build step needed)* |
| **Publish Directory** | `.` |

Render will automatically serve `index.html` at the root URL.

### 4. (Optional) Add a rewrite rule for `/privacy`

If you want the page accessible at `/privacy` (e.g. `https://your-app.onrender.com/privacy`):

1. In the static site settings, scroll to **Redirect/Rewrite Rules**.
2. Click **Add Rule** and enter:

| Source | Destination | Action |
|---|---|---|
| `/privacy` | `/index.html` | **Rewrite** |

> **Tip:** Use **Rewrite** (not Redirect) so the URL stays as `/privacy` in the browser.

### 5. Deploy

Click **Create Static Site**. Render will deploy in about a minute. Your privacy policy will be live at:

```
https://<your-site-name>.onrender.com/
```

### 6. Update the policy page

Open `index.html` and replace the placeholder contact note:

```html
<p class="contact-note"><strong>Contact:</strong> [Your email or contact method — required for compliance]</p>
```

with your actual contact email or method, then commit and push. Render will automatically redeploy.

---

## Local preview

Open `index.html` directly in a browser — no server needed.
