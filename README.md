# Dynamic Dance Website: How to Edit Everything

This is the guide for keeping the Dynamic Dance website up to date. You do **not** need to know how to code.

- **Live site:** https://umdynamic-jpg.github.io
- **Editor (where you make changes):** https://umdynamic-jpg.github.io/admin/
- **Code and history:** https://github.com/umdynamic-jpg/umdynamic-jpg.github.io

**Contents**
1. [Quick start](#1-quick-start)
2. [Getting access](#2-getting-access)
3. [Logging in](#3-logging-in)
4. [A tour of the editor](#4-a-tour-of-the-editor)
5. [Common tasks, step by step](#5-common-tasks-step-by-step)
6. [Photo tips](#6-photo-tips)
7. [Writing page content (Markdown cheat sheet)](#7-writing-page-content-markdown-cheat-sheet)
8. [Undoing a mistake](#8-undoing-a-mistake)
9. [Setting up the contact form](#9-setting-up-the-contact-form)
10. [Troubleshooting](#10-troubleshooting)
11. [Yearly e-board handoff checklist](#11-yearly-e-board-handoff-checklist)
12. [For the site owner: how it all works](#12-for-the-site-owner-how-it-all-works)
13. [Using a custom domain](#13-using-a-custom-domain)
14. [Editing without the dashboard](#14-editing-without-the-dashboard)
15. [Map of the files](#15-map-of-the-files)

---

## 1. Quick start

1. Open https://umdynamic-jpg.github.io/admin/ in **Chrome**.
2. Click **Login with GitHub** and approve the pop-up.
3. Pick a section on the left, change what you want, and click **Publish → Publish now**.
4. Wait **1 to 2 minutes**, then hard-refresh the live site (**Cmd+Shift+R** on Mac, **Ctrl+Shift+R** on Windows).

That's the whole cycle. Everything below is detail.

---

## 2. Getting access

Anyone can open the login page, but only people with **write access** to the repository can save changes.

**To add a new editor (site owner does this):**
1. Go to the repository on GitHub, then **Settings → Collaborators → Add people**.
2. Enter their GitHub username or email and choose **Write** access.
3. They get an email invitation and must **accept it** before they can edit.

**To remove someone** (for example, a graduating member): the same page, click the trash icon next to their name.

Each editor needs their own free GitHub account (github.com). Everyone logging in with their own account means you can see who changed what.

---

## 3. Logging in

1. Go to https://umdynamic-jpg.github.io/admin/
2. Click **Login with GitHub**.
3. A pop-up opens. Click **Authorize** if GitHub asks. The pop-up closes and the editor opens.

**Important if you have more than one GitHub account:** the login uses whichever account is active in your browser. If it's the wrong one, you'll just be sent back to the login screen. Fix it by opening an **Incognito/Private window**, logging into github.com with the right account, then opening the editor in that same window.

**Pop-ups blocked?** Click the blocked-pop-up icon in Chrome's address bar and choose "Always allow."

---

## 4. A tour of the editor

After logging in, you'll see **Site content** with these sections:

| Section | What it controls |
|---|---|
| **Home page** | The big tagline, intro sentence, main button, "Since 2004" sticker, top photo, the three colored boxes, the story, and the Instagram strip |
| **Gallery photos** | Every photo on the Gallery page |
| **Links, email and logo** | The logo, team email, Instagram/TikTok/YouTube links, and the contact form link |
| **Join Us page** | The Join Us page (Opportunities and Workshops sections) |
| **Rip The Floor page** | The Rip The Floor page, including the competition guidelines |

Each section is a form. Edit the fields, then use the **Publish** button at the top.

**What "Publish" does:** It saves your changes directly to the live site's code. There is no draft step, so double-check before publishing. If you slip, see [Undoing a mistake](#8-undoing-a-mistake).

---

## 5. Common tasks, step by step

### Change the home page tagline
1. **Home page → Tagline words**.
2. Edit a word, drag to reorder, or use **Add word** / the trash icon.
3. Keep each word starting with the letter you want highlighted in red. For DYNAMIC, the lines are *Determined. Young. New. Artists. Maintaining. an Incredible. Craft.* The first letter of each line is the red one.

### Change the intro sentence, button text, or sticker
**Home page → Intro sentence / Main button text / Sticker text.** The sticker is the red "Since 2004" badge on the top photo. The button always links to the Join Us page.

### Change the three colored boxes
**Home page → Boxes.** For each box you can change the title, text, which page it links to, and its color (red, black, or white).
Links use the page's file name:
- Join Us page: `join.html`
- Rip The Floor page: `rip-the-floor.html`
- Gallery: `gallery.html`
- Contact: `contact.html`

### Edit the story
**Home page → Story text.** Use blank lines between paragraphs.

### Swap the home page photos
**Home page → Top photo** (or **Story photo**), click the current image, choose **Replace** (or **Choose an image**), then **Upload** a new one. See [Photo tips](#6-photo-tips).

### Add photos to the gallery
1. **Gallery photos → Photos → Add photos**.
2. Click **Choose an image → Upload** and pick the file.
3. Fill in **Description** (one short sentence describing the photo, e.g. "Dynamic performing at Rip The Floor"). This helps people using screen readers.
4. Repeat for each photo, then Publish. Drag items to reorder; use the trash icon to remove one.

### Update social links or the team email
**Links, email and logo.** Paste the full link (starting with `https://`) for Instagram, TikTok, and YouTube. Changes appear in the footer of every page.

### Edit the Join Us or Rip The Floor page
Open the page, change the **Title** if needed, and edit **Page content** in the editor. You can switch between **Rich Text** and **Markdown** with the toggle above the box. Formatting help is in [section 7](#7-writing-page-content-markdown-cheat-sheet).

### Start a new year of Rip The Floor
Open **Rip The Floor page**, change the **Title** (for example to "Rip The Floor 2026"), and update the content. The page address and the menu link stay the same.

### Change the nav menu or add a brand-new page
The dashboard can't do this. See [Editing without the dashboard](#14-editing-without-the-dashboard), or ask whoever maintains the site.

---

## 6. Photo tips

- **File size:** aim for **under 1 MB** per photo, and about **1600 pixels wide** at most. Huge photos make the site slow, especially on phones. Free tools like squoosh.app shrink photos without visible quality loss.
- **File type:** JPG for photos, PNG for the logo or graphics with transparency.
- **File names:** use simple names with dashes and no spaces, like `rtf-2026-finals.jpg`.
- **Where they go:** uploaded photos are saved in the repository's `images` folder.
- **Landscape vs. portrait:** gallery photos are cropped to a 4:3 box, so keep important things away from the edges.
- **Only upload photos you have permission to share publicly.** The repository is public, so anyone can view and download the files.

---

## 7. Writing page content (Markdown cheat sheet)

If you use the Markdown view of a page, this is all you need:

| You type | You get |
|---|---|
| `## Section heading` | A heading (use `##` for sections, `###` for smaller ones) |
| `**bold text**` | **bold text** |
| `*italic text*` | *italic text* |
| `[link text](https://example.com)` | A clickable link |
| `- item` (new line per item) | A bulleted list |
| `1. item` (new line per item) | A numbered list |
| A blank line | Starts a new paragraph |

Rich Text mode has buttons for the same things, so you can ignore Markdown entirely if you prefer.

---

## 8. Undoing a mistake

Every change is saved in history, so nothing is truly lost.

**To see what changed:** go to the repository on GitHub and click the **commits** link (it shows a clock icon and a number like "34 Commits"). Each editor save is one entry.

**To undo the last change:**
1. Open that commit from the commits list.
2. Click the **⋯** menu at the top right and choose **Revert** (this creates a new change that cancels the old one).
3. Click **Create pull request**, then **Merge pull request**, to apply it.

**To restore one file's old text:** open the file on GitHub, click **History**, open an older version, and copy the text back into the editor.

---

## 9. Setting up the contact form

The contact page sends messages through **Formspree**, a free form service.

1. Create an account at formspree.io using the team email.
2. Create a new form and copy its link (it looks like `https://formspree.io/f/abcdwxyz`).
3. In the editor, go to **Links, email and logo → Contact form link** and paste it in. Publish.
4. Send a test message from the live Contact page and confirm it arrives. The first time, Formspree may email you to confirm the address.

The free plan has a monthly limit on messages. If messages stop arriving, check your Formspree dashboard.

---

## 10. Troubleshooting

| Problem | What to try |
|---|---|
| **Login bounces me back to the login screen** | You're probably logged into the wrong GitHub account. Use an Incognito window, log into github.com with the correct account first, then open the editor there. Also confirm you've accepted the collaborator invitation. |
| **Pop-up doesn't appear** | Allow pop-ups for the site in Chrome's address bar. |
| **"Failed to load config.yml (404)"** | Make sure you're at `/admin/` (with the trailing `/admin/`), not the main site. If you are, wait a few minutes and hard-refresh; the site may still be rebuilding. |
| **My change isn't showing on the live site** | Wait 2 minutes, then hard-refresh (Cmd+Shift+R). If it's still missing, open the repository's **Actions** tab and look at the latest run: a green ✓ means it's published, a red ✗ means the build failed (click it to see why), and a yellow circle means it's still running. |
| **Build failed (red ✗)** | Usually caused by a typo in a data file. Revert the last change (see section 8), or ask the site owner. |
| **A photo is broken or missing** | Re-upload it. Check the file name has no spaces or odd characters. |
| **I can log in but can't save** | Your account needs **Write** access to the repository (section 2). |
| **Contact form messages aren't arriving** | Check Formspree (section 9) and make sure the form link in the editor is correct. |
| **A pop-up says "Login failed"** | Close it and try again. If it keeps happening, tell the site owner: the login service secret may need refreshing (section 12). |

---

## 11. Yearly e-board handoff checklist

Do this every time leadership changes:

- [ ] Add the new editors as collaborators (section 2) and **remove** the ones who left.
- [ ] Confirm at least **two people** can log into the editor and save a test change.
- [ ] Share the team logins (GitHub, Cloudflare, Formspree, and the domain registrar if you have a custom domain) through your team's usual password manager, not in chat or email.
- [ ] Make sure the **team email** is the recovery email on every account, so no account depends on one graduating person.
- [ ] Update the Rip The Floor page, the Join Us page, and any dates.
- [ ] Update the gallery with the year's best photos.
- [ ] Re-read this guide and fix anything that's out of date.

---

## 12. For the site owner: how it all works

You don't need this to edit the site. It's here for whoever maintains the setup.

**The pieces**
- **GitHub Pages** hosts the site for free from the repository's `main` branch. It runs **Jekyll** automatically to turn the files into web pages.
- **Decap CMS** is the editor at `/admin/`. It is a web page that edits the repository's files through the GitHub API.
- **A Cloudflare Worker** named `dynamic-auth` (at `https://dynamic-auth.umdynamic.workers.dev`) handles the GitHub login. GitHub Pages can't do logins by itself, so this small free service passes the login result back to the editor.
- **A GitHub OAuth App** named "Dynamic Dance Editor" (under the `umdynamic-jpg` account, in **Settings → Developer settings → OAuth Apps**) lets the editor ask GitHub who you are.
- **Formspree** receives contact-form messages.

**Where the settings live**
- `admin/config.yml`: tells the editor which repo to edit (`umdynamic-jpg/umdynamic-jpg.github.io`), which branch (`main`), and the login service address (`base_url`). It also defines the editor's forms.
- Cloudflare worker, **Settings → Variables and Secrets**: `GITHUB_CLIENT_ID` and `GITHUB_CLIENT_SECRET`. These come from the OAuth App.
- OAuth App settings: homepage `https://umdynamic-jpg.github.io`, callback URL `https://dynamic-auth.umdynamic.workers.dev/callback`.

**If the GitHub account or repository name ever changes**
1. Rename or move the repo (for a user site it must be named `ACCOUNT.github.io`).
2. Update `repo:` in `admin/config.yml`.
3. Update the OAuth App homepage URL to the new site address. Consider recreating the OAuth App under the new account, then put the new Client ID and secret into the Cloudflare worker and redeploy.

**If the login stops working suddenly:** generate a new client secret in the OAuth App, update `GITHUB_CLIENT_SECRET` in Cloudflare, and click **Deploy**.

**Security notes**
- Never share the client secret or put it in the repository.
- The repository is public, so don't put private information in any file.
- Only collaborators with Write access can change the site, even though anyone can see the login page.

**Before cancelling Squarespace**
- The logo and the two home-page photos currently load from Squarespace's servers. **Download them and re-upload them through the editor** (**Links, email and logo → Logo**, and **Home page → Top photo / Story photo**) before the Squarespace plan ends, or they will disappear.
- Check every page and link on the new site, and set up the contact form (section 9).
- If you use a Squarespace-registered domain, plan the transfer carefully (section 13).

---

## 13. Using a custom domain

The free address is `umdynamic-jpg.github.io`. A custom domain (like `umdynamicdance.com`) costs about $12 to $20 per year at a registrar.

1. Buy or transfer the domain at a registrar. Transfers can take days and may be blocked for a period after a recent registration or transfer.
2. In the repository, go to **Settings → Pages → Custom domain**, enter the domain, and save. Turn on **Enforce HTTPS** when it becomes available.
3. At your registrar's DNS settings, add the records GitHub tells you to. For the main domain these are normally four `A` records pointing to GitHub's addresses, plus a `CNAME` record for `www` pointing to `umdynamic-jpg.github.io`. **Check GitHub's current "Managing a custom domain for your GitHub Pages site" documentation for the exact values**, since they can change.
4. DNS changes can take from minutes to a day to take effect.
5. Then update the OAuth App's homepage URL to the new address. Because the editor and login service use fixed addresses, check the login again after the switch.

---

## 14. Editing without the dashboard

If the editor is ever down, or you need to change something it can't, you can edit files directly on GitHub:

1. Open the file in the repository and click the **pencil icon**.
2. Make your change and click **Commit changes**.
3. Wait for the green ✓ in the Actions tab.

Be careful with the first few lines of a file that sit between two lines of `---`. They're settings, and a typo there can break the page.

**Adding a menu item or a new page:** create a new file (for example `events.md`) in the top level of the repository, copying the layout lines from `join.md`, then add the page to the `nav` line in `_layouts/default.html`. To make it editable in the dashboard, also add an entry for it in `admin/config.yml`. If this feels like too much, ask someone comfortable with code.

---

## 15. Map of the files

| File or folder | What it is | Edit in the dashboard? |
|---|---|---|
| `_data/home.yml` | Home page text, photos, and boxes | Yes: **Home page** |
| `_data/gallery.yml` | Gallery photo list | Yes: **Gallery photos** |
| `_data/settings.yml` | Logo, email, social links, contact form link | Yes: **Links, email and logo** |
| `join.md` | Join Us page | Yes: **Join Us page** |
| `rip-the-floor.md` | Rip The Floor page | Yes: **Rip The Floor page** |
| `contact.html` | Contact page layout | No (text is fixed, form link is in settings) |
| `gallery.html` | Gallery page layout | No (photos come from `gallery.yml`) |
| `index.html` | Home page layout | No |
| `_layouts/` | Page templates (menu, header, footer) | No |
| `style.css` | Colors, fonts, and spacing | No |
| `script.js` | Scroll effects and animations | No |
| `images/` | Uploaded photos | Yes, through any photo field |
| `admin/` | The editor itself and its settings (`config.yml`) | No |
| `_config.yml` | Site title and description | No |

**Rule of thumb:** if you're not sure whether to change a file, use the dashboard instead, and leave everything else alone.
