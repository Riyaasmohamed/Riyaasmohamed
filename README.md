# GitHub setup – step by step (about 30 minutes)

Account: **https://github.com/Riyaasmohamed**
Everything to upload is in this `github/` folder. Copy it to your laptop first (WinSCP: drag `github` to the left panel).

```
github/
├── Riyaasmohamed/      → your profile page (README + snake animation)
├── banking-api/        → new Spring Boot banking project
├── riyaas-portfolio/   → the 3D portfolio (Angular + Spring Boot)
└── profile-preview.png → how your profile page will look
```

---

## Step 0 – Security first (2 min)
1. **Settings → Password and authentication → Change password.**
2. Same page → **Enable two-factor authentication** (use the GitHub Mobile app or Google Authenticator).
3. Never share your password with anyone.

## Step 1 – Profile settings (5 min)
Click your photo (top right) → **Settings → Public profile**:

| Field | Put this |
|---|---|
| Profile picture | A clear, smiling headshot, plain background |
| Name | `Riyaas Mohamed` |
| Bio | `Java Backend Developer · Spring Boot, Microservices, MySQL · ~2 yrs building banking APIs · Open to work` |
| URL | `https://riyaas-mohamed.netlify.app` |
| Social accounts | `https://linkedin.com/in/riyaasmohamedn` |
| Company | leave empty (keeps your job search quiet) |
| Location | `Bengaluru, India` |

Click **Update profile**.
Then on the same page → **Contributions & activity** → tick **Include private contributions on my profile** → Save.

## Step 2 – Profile README (the big banner page) (5 min)
1. Top right **+ → New repository**.
2. Repository name: **`Riyaasmohamed`** (exactly your username). GitHub shows "✨ special repository" – good.
3. **Public**, tick **Add a README file** → **Create repository**.
4. Click `README.md` → ✏️ (Edit) → delete everything → open `Riyaasmohamed/README.md` from this folder in Notepad → copy all → paste → **Commit changes**.
5. **Add file → Create new file**. In the name box type: `.github/workflows/snake.yml`
   Open `Riyaasmohamed/.github/workflows/snake.yml` in Notepad → copy all → paste → **Commit changes**.
6. Go to **Settings → Actions → General → Workflow permissions** → choose **Read and write permissions** → Save.
7. **Actions** tab → **Contribution snake** → **Run workflow** → Run. Wait 1–2 minutes until it is green ✅.
8. Open **https://github.com/Riyaasmohamed** – you will see the banner page.

## Step 3 – Upload `banking-api` (5 min)
1. **+ → New repository** → name **`banking-api`**.
   Description: `Multi-tenant banking REST API – maker-checker, idempotent transfers, JWT, audit trail (Spring Boot)`
   **Public**. Do **not** tick "Add a README". → **Create repository**.
2. On the empty repo page click the link **"uploading an existing file"**.
3. Open the `banking-api` folder on your laptop, select **everything inside it** (Ctrl+A – including the `.github` folder) and drag it onto the page.
4. Commit message: `Initial commit: banking API` → **Commit changes**.
5. Open the **Actions** tab – the **CI** build runs automatically and turns green ✅ (the badge in the README turns green too).
6. On the repo page, right side **About ⚙️**:
   - Website: `https://riyaas-mohamed.netlify.app`
   - Topics: `java` `spring-boot` `spring-security` `jwt` `rest-api` `banking` `fintech` `multi-tenancy` `jpa` `docker`
   - Save.

## Step 4 – Upload `riyaas-portfolio` (5 min)
Same as Step 3 with:
- Name: **`riyaas-portfolio`**
- Description: `My 3D developer portfolio – Angular + three.js frontend, Spring Boot API`
- Upload **everything inside** the `riyaas-portfolio` folder.
- About ⚙️ → Website: `https://riyaas-mohamed.netlify.app` · Topics: `portfolio` `angular` `threejs` `spring-boot` `java`

## Step 5 – Pin your best work (1 min)
Go to **https://github.com/Riyaasmohamed** → **Customize your pins** → tick **banking-api** and **riyaas-portfolio** → Save.

## Step 6 – Update the live website (2 min)
The website now has a **GitHub** button and the new Banking API project.
Netlify → your project → **Deploys** → drag the folder `portfolio/website-upload` onto the page. Same link, updated site.

---

### Keep it alive
- Push small, real improvements every week (e.g. add PostgreSQL + Flyway to banking-api, add a test). A steady green contribution graph looks much better than a burst.
- Never upload company code, configs or passwords.
