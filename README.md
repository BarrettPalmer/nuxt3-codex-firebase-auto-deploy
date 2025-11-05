# Nuxt 3 + Codex + Firebase Hosting Setup (For Beginners)

This guide shows you how to:
- Set up GitHub and VS Code
- Install and use Codex CLI
- Create a Nuxt 3 site
- Deploy automatically with Firebase Hosting
- Push code using VS Code GUI (no terminal)
- Connect your custom domain

Everything is step-by-step, no experience required.

---

## 1. Create a GitHub Account
1. Visit [github.com](https://github.com)
2. Click “Sign up”
3. Fill out your info
4. Confirm your email

---

## 2. Install Visual Studio Code (VS Code)
1. Go to [code.visualstudio.com](https://code.visualstudio.com)
2. Download and install it
3. Open VS Code

---

## 3. Install GitHub Plugin in VS Code
1. Open VS Code
2. Click the **Extensions** tab (left sidebar)
3. Search for `GitHub Pull Requests and Issues`
4. Click **Install**

---

## 4. Sign In to GitHub from VS Code
1. Press `Ctrl+Shift+P` (or `Cmd+Shift+P`)
2. Type `GitHub: Sign in`
3. Press Enter
4. A browser opens. Log in to GitHub and allow access
5. Done — your GitHub is now connected to VS Code

---

## 5. Clone Your Repository (No Terminal)
1. In VS Code:
   - Open Command Palette (`Ctrl+Shift+P`)
   - Type `Git: Clone` and hit Enter
   - Paste your GitHub repo link (example: `https://github.com/your-username/my-nuxt-site`)
2. Choose a folder where to save the files
3. Open the folder when prompted

---

## 6. Install Codex CLI
1. Open terminal in VS Code (Terminal > New Terminal)
2. Run:
   ```
   npm install -g @openai/codex
   ```
3. Then:
   ```
   codex --login
   ```
4. Sign in with ChatGPT when prompted

---

## 7. Set Up Nuxt 3
1. In terminal:
   ```
   npx nuxi init .
   npm install
   ```
2. To run the site locally:
   ```
   npm run dev
   ```

---

## 8. Use Codex CLI to Build Pages
1. Create a file: `instructions.md`
2. Write in plain English what you want (e.g. homepage, contact form)
3. Run:
   ```
   codex
   ```
4. Enter your request. Codex will build the code into your folder.

---

## 9. Install Firebase CLI
1. In terminal:
   ```
   npm install -g firebase-tools
   firebase login
   ```
2. In VS Code terminal:
   ```
   firebase init hosting
   ```
3. Choose:
   - Existing Firebase project
   - Public directory: `.output/public`
   - Configure as SPA: Yes
4. Don’t overwrite existing files

---

## 10. Connect Firebase to GitHub (Auto Deploy)
1. Run:
   ```
   firebase init hosting:github
   ```
2. Choose your GitHub repo and branch (usually `main`)
3. Firebase adds `.github/workflows` file
4. Now, when you push to GitHub, Firebase will deploy your site

---

## 11. Push Your Code Using VS Code (Not Terminal)
1. Make sure your folder is open in VS Code
2. Click the **Source Control** icon on the sidebar
3. Type a commit message (example: `initial commit`)
4. Click the checkmark to commit
5. Click **Publish Branch** to push your code to GitHub

---

## 12. Connect a Custom Domain (Firebase)
1. Go to [console.firebase.google.com](https://console.firebase.google.com)
2. Choose your project
3. Click **Hosting**
4. Click **Add custom domain**
5. Enter your domain (example: `yourdomain.com`)
6. Firebase will give you DNS records
7. Log in to your domain registrar (GoDaddy, Namecheap, etc.)
8. Update DNS settings with the Firebase records
9. Wait for DNS to update (can take a few minutes to a few hours)
10. Your Nuxt site will now work on your domain

---

You’re done. Push code, Codex builds it, Firebase deploys it.
