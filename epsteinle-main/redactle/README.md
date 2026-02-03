# Daily Redactle Game

A daily word-guessing game where players reveal hidden passages by guessing words, similar to Redactle.

## 🚀 Deploy to Vercel (Free)

### Method 1: Drag & Drop (Easiest)

1. Go to [vercel.com](https://vercel.com)
2. Sign up for free (use GitHub, GitLab, or email)
3. Click "Add New..." → "Project"
4. Drag the entire `redactle-game` folder into the upload area
5. Click "Deploy"
6. Done! Your game is live at `your-project.vercel.app`

### Method 2: GitHub Integration (Recommended for updates)

1. Create a GitHub account if you don't have one
2. Create a new repository called `redactle-game`
3. Upload `index.html` and `passages.json` to the repository
4. Go to [vercel.com](https://vercel.com) and sign in
5. Click "Add New..." → "Project"
6. Import your GitHub repository
7. Click "Deploy"

**Updating daily passages with GitHub:**
- Go to your repository on GitHub
- Click on `passages.json`
- Click the pencil icon to edit
- Update your passages
- Commit changes
- Vercel automatically redeploys!

## 📝 How to Update Daily Passages

Edit the `passages.json` file. Each passage needs:

```json
{
  "text": "Your passage text goes here. Can be multiple sentences.",
  "source": "Where this passage is from",
  "date": "2024-01-01"
}
```

### Example:

```json
{
  "passages": [
    {
      "text": "The quick brown fox jumps over the lazy dog. This sentence contains every letter of the alphabet at least once.",
      "source": "Pangram Example",
      "date": "2024-01-01"
    },
    {
      "text": "Another passage for day 2.",
      "source": "Day 2 Source",
      "date": "2024-01-02"
    }
  ]
}
```

## 🎮 How the Game Works

1. **Daily Rotation**: The game automatically selects a different passage each day
2. **Common Words**: Articles (the, a, an) and common words are always visible
3. **Guessing**: Players guess words to reveal them
4. **Clicking**: Players can click redacted words to reveal them (counts as a guess)
5. **Stats**: Tracks guesses, percentage revealed, and accuracy
6. **Completion**: Shows source when all words are revealed

## 🔄 Daily Updates

The game uses the current date to determine which passage to show. It cycles through your passages in order:
- Day 1 → Passage 1
- Day 2 → Passage 2
- Day 3 → Passage 3
- Day 4 → Back to Passage 1 (if you only have 3)

Add as many passages as you want to the array!

## ✏️ Tips for Good Passages

- **Length**: 50-200 words works best
- **Variety**: Mix topics to keep it interesting
- **Difficulty**: Longer, more complex words make it harder
- **Sources**: Always credit your sources

## 🛠️ File Structure

```
redactle-game/
├── index.html       (The game - don't edit unless you know what you're doing)
├── passages.json    (Your daily passages - edit this!)
└── README.md        (This file)
```

## 🆘 Troubleshooting

**Game shows "Error Loading Puzzle":**
- Check that `passages.json` is in the same folder as `index.html`
- Verify your JSON is valid (use jsonlint.com)
- Make sure you have at least one passage

**Passage not updating:**
- Clear your browser cache
- The game changes at midnight UTC

**Want to test locally:**
- You can't open `index.html` directly (CORS issues)
- Use a local server or just deploy to Vercel to test

## 📧 Need Help?

If you run into issues:
1. Check that your JSON is valid
2. Make sure both files are uploaded
3. Try redeploying on Vercel
4. Check the browser console for errors (F12)

Enjoy your daily Redactle game! 🎉
