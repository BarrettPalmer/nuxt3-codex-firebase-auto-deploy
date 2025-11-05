# Full Beginner Guide: Nuxt 3 + Codex + Firebase Hosting
Your Prompt to (ChatGPT):

I want you to create an AI prompt for Codex.
I'm using VS Code.
I want Codex to build a Nuxt 3 website using Tailwind CSS and Firebase Hosting.
I want it to start from scratch: install dependencies, initialize the project, and build it.
Use this URL as design inspiration: https://example.com

## 1. Create a GitHub Account
1. Go to github.com
2. Click "Sign up"
3. Choose username, email, password
4. Confirm email

## 2. Install VS Code
1. Visit code.visualstudio.com
2. Download and install
3. Open VS Code

## 3. Install Codex CLI
1. Open terminal
2. Run:
   npm install -g @openai/codex
3. Then:
   codex --login
4. Sign in with your ChatGPT account

## 4. Set Up GitHub Repo
1. On GitHub, click "New repository"
2. Name it, e.g., `my-nuxt-site`
3. Create repository
4. In VS Code:
   - Open Command Palette
   - Run Git: Clone
   - Paste your GitHub repo URL
   - Open the folder

## 5. Use Codex to Generate Project
1. In VS Code terminal, run:
   codex
2. Tell Codex to build the project, for example:
   "Create a Nuxt 3 site with a home page and about page using Tailwind CSS."

## 6. Firebase Hosting Setup
1. Install Firebase CLI:
   npm install -g firebase-tools
2. Login:
   firebase login
3. Init hosting:
   firebase init hosting
4. Choose:
   - Existing project
   - Public dir: `.output/public`
   - SPA: Yes

## 7. GitHub Deploy Setup
1. Run:
   firebase init hosting:github
2. Choose repo + branch
3. GitHub Actions config will be added

## 8. Push with VS Code
1. Click Source Control in VS Code
2. Commit message
3. Click ✓ to commit
4. Click Publish Branch

## 9. Add Domain in Firebase
1. Go to Hosting in Firebase console
2. Click Add Custom Domain
3. Follow DNS steps from your registrar

You're live.
