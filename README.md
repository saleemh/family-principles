
# Family Principles (Hussain) — README

A simple, transparent way for our family to **propose**, **discuss**, and **update** our shared principles using GitHub pull requests (PRs).

- 📄 **Main file:** `Hussain Family Principles.md`  
- 🔒 **Branch protection:** `main` is protected — all changes require a PR + parent approval  
- 👪 **Reviewers:** Parents are CODEOWNERS; at least one parent must approve  
- 🧭 **Council:** We announce merged changes at the weekly Family Council  

---

## 📱 How Kids Can Propose Changes (Phone-Friendly)

### Using GitHub Mobile App (recommended)
1. Install the **GitHub app** (iOS/Android) and **sign in**.  
2. Open the `family-principles` repo → tap **⋯ → Fork**.  
3. In your **fork**, open `Hussain Family Principles.md`.  
4. Tap the **✏️ pencil** to edit. Make your wording change (focus on one idea).  
5. Tap **Commit changes** → add a short message like:  
   `Proposal: adjust weekday screen time`.  
6. The app suggests **Compare & pull request** → tap it.  
7. Fill the PR form (title + description). Use this format:

   ```
   Before
   > (paste the current text)

   After
   > (paste your new text)

   Why
   > (1–2 lines: why this helps — fairness, clarity, sleep, etc.)
   ```

8. Tap **Create pull request**. Done! A parent will review.  

### Using GitHub Mobile Website
1. Log into github.com → open `family-principles` → **Fork**.  
2. In your fork, open `Hussain Family Principles.md` → tap **✏️ Edit**.  
3. Commit → then **Contribute → Open pull request**.  
4. Fill out the “Before / After / Why” blocks.  

---

## 👨‍👩‍👧 How Parents Review and Merge

### Prerequisites
- `main` branch has **classic branch protection** (PR required, 1 approval, require CODEOWNERS).  
- `.github/CODEOWNERS` lists parents’ usernames, e.g.:  
  ```
  * @saleem @maureen
  ```

### Reviewing in GitHub App
1. Open the **Pull Requests** tab → select the child’s PR.  
2. Read the **Conversation**, then tap **Files changed**.  
3. Tap **+** to add comments on specific lines (be kind, specific).  
4. Tap **Review** → choose:  
   - **Request changes** (needs edits),  
   - **Approve** (ready to merge), or  
   - **Comment** (questions only).  
5. If changes requested: child edits → commits again → PR updates automatically.  
6. Once approved, tap **Merge** → choose **Squash & merge** → **Confirm**.  
7. (Optional) **Delete branch** after merge.  

### Reviewing on GitHub Website
1. Go to the PR → **Files changed** → add comments.  
2. Click **Review changes** → **Request changes** / **Approve** / **Comment**.  
3. Merge via **Squash and merge** → Confirm.  

---

## ✅ Etiquette & Expectations
- **Respect first.** Polite, constructive language only.  
- **Be specific.** Always show exact “Before → After” text.  
- **Small scope.** One change per PR when possible.  
- **No personal info.** Don’t include school names, addresses, or phone numbers.  

---

## 🛠 Troubleshooting
- **Can’t see edit pencil?** You’re in the main repo. Edit in **your fork**.  
- **No parent review required?** CODEOWNERS file needs fixing.  
- **PR didn’t auto-suggest?** In your fork, tap **Contribute → Open pull request**.  

---

## 📂 Repo Files
- `Hussain Family Principles.md` — the document we edit.  
- `.github/CODEOWNERS` — requires parent review.  
- `.github/PULL_REQUEST_TEMPLATE.md` — pre-fills “Before / After / Why.”  
- `CONTRIBUTING.md` — full contributor guide.  

---

## 🗓 Weekly Council
Approved changes are announced at **Sunday Family Council**, then trialed or made permanent.  

---

## ⚡ Optional: Parent Power Users (CLI)
```bash
# Install GitHub CLI (macOS): brew install gh

# List open PRs
gh pr list

# Review a PR
gh pr review <number> --approve
gh pr review <number> --request-changes --body "Please clarify bedtime rule"

# Merge with squash and delete branch
gh pr merge <number> --squash --delete-branch
```
