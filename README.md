# Dear Damsels – Static Landing Page

A single-page “thank you” site that replaces the former WordPress installation at **deardamsels.com**.  
Built with plain HTML/CSS, served by **GitHub Pages**, and intended to stay online until the domain expires (October 2026).

&nbsp;

## ✨ Live site

<https://deardamsels.com> &nbsp;|&nbsp; <https://www.deardamsels.com>

&nbsp;

## 📂 Project structure

/
├── index.html   # main page shown at /
├── 404.html     # catch-all redirect → /
├── logo.png     # placeholder; drop real logo here
├── .nojekyll    # disable Jekyll processing
└── CNAME        # tells GitHub Pages the custom domain

&nbsp;

## 🚀 Quick-start (local → GitHub Pages)

```bash
# 1 — clone the repo or initialise a new one, then drop these files in
git init
git add .
git commit -m "Initial Dear Damsels landing page"

# 2 — push to a GitHub repo called deardamsels-landing
git remote add origin git@github.com:YOUR-USER/deardamsels-landing.git
git branch -M main
git push -u origin main

	1.	Open the repo on GitHub → Settings → Pages.
	2.	Select Branch: main / (root) → Save.
	3.	In Custom domain, enter deardamsels.com → Save.
	4.	Wait a few minutes for the green HTTPS padlock.

DNS records (already set at the registrar):

A  @   185.199.108.153
A  @   185.199.109.153
A  @   185.199.110.153
A  @   185.199.111.153
CNAME  www  YOUR-USER.github.io
```

🔄 Catch-all redirect (404.html)

GitHub Pages serves 404.html for every unknown path.
Because we have no other pages, the file uses a meta-refresh and JavaScript to send users straight back to /, ensuring old WordPress URLs land on the new message.

🛠️ Customising
	•	logo.png – replace with the real Dear Damsels logo (keep the filename).
	•	index.html – adjust copy or styling if needed (inline CSS for zero dependencies).
	•	404.html – update the fallback text if you change the site copy.

📄 License

MIT – feel free to reuse this tiny setup for your own projects.

⸻

Maintained by the go.digital team for Dear Damsels. Last updated May 2025.

