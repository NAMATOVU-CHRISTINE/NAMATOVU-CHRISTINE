# 🚀 GitHub Profile Enhancement Setup Guide

This guide will help you set up all the automated features in your enhanced GitHub profile.

## 📋 Prerequisites

- A GitHub account
- Repository named `NAMATOVU-CHRISTINE` (same as your username)
- GitHub Actions enabled in your repository

## 🔧 Setup Steps

### 1. Enable GitHub Actions

1. Go to your repository settings
2. Navigate to **Actions** → **General**
3. Under "Workflow permissions", select **Read and write permissions**
4. Check **Allow GitHub Actions to create and approve pull requests**
5. Click **Save**

### 2. Snake Animation Setup

The snake animation is already configured! It will:
- Run daily at midnight
- Generate a contribution graph animation
- Store it in the `output` branch

**No additional setup required** - just wait for the first run or trigger it manually:
1. Go to **Actions** tab
2. Select **Generate Snake Animation**
3. Click **Run workflow**

### 3. WakaTime Integration (Optional)

To show your coding activity stats:

1. Sign up at [WakaTime](https://wakatime.com/)
2. Install WakaTime plugin in your IDE (VS Code, PyCharm, etc.)
3. Get your API key from [WakaTime Settings](https://wakatime.com/settings/account)
4. Add it to your repository secrets:
   - Go to **Settings** → **Secrets and variables** → **Actions**
   - Click **New repository secret**
   - Name: `WAKATIME_API_KEY`
   - Value: Your WakaTime API key
   - Click **Add secret**

### 4. Recent Activity Setup

The recent activity workflow is configured to update every 6 hours automatically.

**First run:**
1. Go to **Actions** tab
2. Select **Update Recent Activity**
3. Click **Run workflow**

### 5. Profile Stats Customization

You can customize the stats widgets by editing the URLs in `README.md`:

#### GitHub Stats Card
```markdown
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=NAMATOVU-CHRISTINE&show_icons=true&theme=radical)
```

**Customization options:**
- `theme`: radical, dark, default, tokyonight, onedark, cobalt, etc.
- `hide`: comma-separated list of metrics to hide (stars, commits, prs, issues)
- `show_icons`: true/false
- `count_private`: true/false

#### Language Stats
```markdown
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=NAMATOVU-CHRISTINE&layout=compact&theme=radical)
```

**Customization options:**
- `layout`: compact, normal
- `langs_count`: number of languages to show (default: 5)
- `hide`: comma-separated list of languages to hide

### 6. Adding Real Project Cards

Replace the placeholder repository names in the Featured Projects section:

```markdown
[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=NAMATOVU-CHRISTINE&repo=YOUR-REPO-NAME&theme=radical)]
```

Replace `YOUR-REPO-NAME` with your actual repository names.

## 🎨 Customization Tips

### Color Schemes

Current theme uses:
- Primary: `#0FA90F` (green)
- Secondary: `#ffd700` (gold)
- Background: `#0D1117` (dark)

To change colors, search and replace these hex codes in `README.md`.

### Adding More Badges

Visit [Shields.io](https://shields.io/) or [Simple Badges](https://badges.pages.dev/) to create custom badges.

Example:
```markdown
![Custom Badge](https://img.shields.io/badge/Your_Text-Your_Color?style=for-the-badge&logo=your-logo&logoColor=white)
```

### Adding Social Links

Add more social platforms in the "Let's Connect" section:

```markdown
<a href="YOUR_PROFILE_URL">
  <img src="https://img.shields.io/badge/Platform_Name-Color?style=for-the-badge&logo=platform&logoColor=white" />
</a>
```

## 🔄 Updating Content

### Blog Posts

Edit `BLOG_POSTS.json` to update your blog posts:

```json
{
  "posts": [
    {
      "title": "Your Post Title",
      "slug": "https://your-blog.com/post-url",
      "date": "2025-01-15",
      "category": "Category",
      "emoji": "🔥"
    }
  ]
}
```

### Projects

Edit `PROJECTS.md` to update your featured projects.

### Collaborators

Edit `COLLABORATORS.md` to update collaboration information.

## 🐛 Troubleshooting

### Snake animation not showing
- Check if the workflow ran successfully in Actions tab
- Verify the `output` branch exists
- Wait 24 hours for the first automatic run

### Stats not updating
- Ensure GitHub Actions has write permissions
- Check workflow logs for errors
- Verify your username is correct in all URLs

### WakaTime not showing
- Verify API key is correct
- Ensure WakaTime plugin is active in your IDE
- Check if you have coding activity in the last 7 days

## 📚 Resources

- [GitHub Profile README Generator](https://rahuldkjain.github.io/gh-profile-readme-generator/)
- [Awesome GitHub Profile README](https://github.com/abhisheknaiidu/awesome-github-profile-readme)
- [GitHub Readme Stats](https://github.com/anuraghazra/github-readme-stats)
- [Shields.io](https://shields.io/)

## 🎉 You're All Set!

Your enhanced GitHub profile is now ready! The automated workflows will keep your profile updated with:
- ✅ Latest contribution activity
- ✅ Animated contribution graph
- ✅ Coding statistics (if WakaTime is set up)
- ✅ Recent GitHub activity

---

**Need help?** Open an issue in this repository or reach out via the contact methods in your profile!
