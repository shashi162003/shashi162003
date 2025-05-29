# 🐍 Snake Animation Setup Guide

## Why the Snake Animation Isn't Working Yet

The snake animation requires a GitHub Actions workflow to run and generate the SVG files. Here's how to fix it:

## 🚀 Steps to Enable Snake Animation

### 1. **Commit and Push the Files**
```bash
git add .
git commit -m "Add snake animation workflow and update README"
git push origin main
```

### 2. **Enable GitHub Actions (if not already enabled)**
- Go to your repository on GitHub
- Click on the **"Actions"** tab
- If prompted, click **"I understand my workflows, go ahead and enable them"**

### 3. **Manually Trigger the Workflow**
- Go to **Actions** tab in your repository
- Click on **"Generate Snake Animation"** workflow
- Click **"Run workflow"** button
- Select **"main"** branch and click **"Run workflow"**

### 4. **Wait for Completion**
- The workflow should complete in 2-3 minutes
- You'll see a green checkmark when it's done
- The snake animation files will be created in the `output` branch

### 5. **Verify the Animation**
- Check if the `output` branch was created
- The snake animation should now appear in your README

## 🔧 Alternative: Quick Fix with Direct SVG

If the workflow doesn't work immediately, you can temporarily use this direct approach:

1. **Replace the snake animation section in README.md with:**

```markdown
### 🐍 Watch My Contributions Get Eaten!

<div align="center">
  <img src="https://github.com/Platane/snk/raw/output/github-contribution-grid-snake.svg" alt="Snake animation" />
</div>
```

## 🎯 Troubleshooting

### If the workflow fails:
1. **Check repository permissions:**
   - Go to Settings → Actions → General
   - Ensure "Read and write permissions" is selected
   - Save changes

2. **Check branch name:**
   - Make sure your default branch is named `main` (not `master`)
   - Update the workflow file if needed

3. **Manual workflow run:**
   - Go to Actions tab
   - Find "Generate Snake Animation"
   - Click "Run workflow" manually

## ✅ Expected Result

Once working, you'll see:
- A cool snake eating your GitHub contributions
- Animation updates automatically every 12 hours
- Different themes for light/dark mode

## 🆘 Still Not Working?

If you're still having issues:
1. Check the Actions tab for error messages
2. Ensure your repository is public (private repos need GitHub Pro)
3. Try the alternative direct SVG approach above
4. The fallback snake GIF will show until the animation is ready

---

**Note:** The snake animation may take a few minutes to appear after the first workflow run. Be patient! 🐍✨
