# Deploying this site to GitHub Pages

Two easy options to publish a free link:

1) Quick — upload via GitHub web UI
   - Create a new **public** repository on GitHub (RepoName).
   - In the repo, click **Add file → Upload files** and drag/drop `index.html`.
   - Commit. Go to **Settings → Pages → Source**, choose branch `main` and `/ (root)`, Save.
   - Site will be available at: `https://USERNAME.github.io/RepoName/`.

2) From your Mac (recommended if you want CLI control)
   - Install Xcode command line tools if needed:
     ```bash
     xcode-select --install
     ```
   - Then run:
     ```bash
     cd ~/Desktop/My\ Website
     git init
     git add .
     git commit -m "Initial site"
     # create a repo on GitHub and copy its HTTPS URL, then:
     git remote add origin https://github.com/USERNAME/RepoName.git
     git branch -M main
     git push -u origin main
     ```
   - Enable Pages in the repository settings as above.

Notes:
- Use `index.html` for the root URL. If you keep another filename, the URL will include that filename.
- If you want, I can create the repo and push for you if you install the Xcode tools or install `gh` and authenticate.
