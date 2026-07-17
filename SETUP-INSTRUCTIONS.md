# Maya Car Accessories — Website Setup Guide

Follow these steps in order. No coding needed — just clicking and uploading.

---

## STEP 1 — Create a GitHub account (storage for your website files)

1. Go to **github.com/signup**
2. Use email: `anh.mehra@gmail.com`
3. Set a password (save it somewhere safe)
4. Verify the email

## STEP 2 — Create a new repository (a project folder on GitHub)

1. Once logged in, click the **+** icon (top right) → **New repository**
2. Name it: `maya-car-accessories`
3. Keep it **Public**
4. Click **Create repository**
5. On the next page, click **"uploading an existing file"**
6. Drag in **everything inside this folder** (all files and the `admin` and `images` folders) — you can select multiple files/folders at once
7. Scroll down, click **Commit changes**

## STEP 3 — Connect Netlify (this makes the site live)

1. Go to **app.netlify.com**
2. Click **Sign up** → **Sign up with GitHub** (use the same GitHub account)
3. Click **Add new site** → **Import an existing project** → **GitHub**
4. Pick the `maya-car-accessories` repository
5. Leave all settings as default (no build command needed) → click **Deploy**
6. In about a minute, you'll get a live link like `random-name-123.netlify.app`
   - Optional: In **Site settings → Change site name**, rename it to something like `maya-car-accessories` so the link becomes `maya-car-accessories.netlify.app`

**Your website is now live at that link. Test it — open it and check everything works.**

## STEP 4 — Turn on the admin login (so your client can edit content)

1. In Netlify, open your site → go to **Site configuration → Identity**
2. Click **Enable Identity**
3. Under **Registration**, set it to **Invite only** (so random people can't sign up)
4. Scroll to **Services → Git Gateway** → click **Enable Git Gateway**
5. Go to the **Identity** tab (top) → click **Invite users**
6. Enter the client's email: `anh.mehra@gmail.com` → send invite
7. The client will get an email — they click the link, set a password, and they're in

## STEP 5 — Client edits the website

1. Client goes to: `your-site-name.netlify.app/admin`
2. Logs in with the email/password from the invite
3. Sees a simple form:
   - **Shop Details** — phone numbers, address, timing, homepage text
   - **Products** — add, remove, or edit any product photo/name/category
   - **Work Videos** — add, remove, or edit video clips
4. Client clicks **Publish** after any change
5. Within a minute or two, the live website updates automatically

---

## Notes
- The design (3D effects, layout, colors) is locked — only content (text, photos, videos, product list) is editable. That's intentional, so the site can't accidentally break.
- If something ever needs a design change (new section, different colors, etc.), that still needs to come back through Claude/a developer — the CMS only handles content.
- Keep video clips short (under ~20 seconds) and small in file size — large videos can slow the site down or fail to upload through the admin panel.
