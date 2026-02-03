# 🚀 Quick Start - Get Your Game Live in 5 Minutes

## Step 1: Download Your Files
You should have these files:
- `index.html` (the game)
- `passages.json` (your content)

## Step 2: Deploy to Vercel

### Option A: Drag & Drop (Fastest)
1. Go to https://vercel.com
2. Click "Sign Up" (use GitHub or email - it's free)
3. After signing in, click "Add New..." button
4. Select "Project"
5. **Drag your entire folder** into the upload area
6. Click "Deploy"
7. ✅ Done! You'll get a URL like `your-game.vercel.app`

### Option B: Via GitHub (Best for daily updates)
1. Go to https://github.com and sign up (free)
2. Click "New repository"
3. Name it `redactle-game`
4. Upload `index.html` and `passages.json`
5. Go to https://vercel.com and sign in
6. Click "Add New..." → "Project"
7. Click "Import" next to your GitHub repo
8. Click "Deploy"
9. ✅ Done!

## Step 3: Update Daily Content

### If you used Drag & Drop:
1. Edit `passages.json` on your computer
2. Go to your Vercel dashboard
3. Click your project
4. Drag the updated `passages.json` into the Files section
5. Vercel auto-redeploys!

### If you used GitHub:
1. Go to your GitHub repository
2. Click `passages.json`
3. Click the pencil icon (Edit)
4. Make your changes
5. Click "Commit changes"
6. Vercel automatically updates your site!

## Adding New Passages

Open `passages.json` and add to the array:

```json
{
  "passages": [
    {
      "text": "Your first passage here.",
      "source": "Where it's from",
      "date": "2024-01-01"
    },
    {
      "text": "Your second passage here.",
      "source": "Where it's from",
      "date": "2024-01-02"
    }
  ]
}
```

⚠️ **Important**: 
- Keep the JSON format exact (commas, quotes, brackets)
- Test at https://jsonlint.com if you get errors
- The game picks passages by day automatically

## That's It!

Your game will:
- Show a different passage each day automatically
- Track player stats
- Look professional
- Work on mobile and desktop
- Cost $0 to host

Share your URL with friends! 🎉
