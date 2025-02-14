## My GitHub Stats

[![My GitHub Stats](https://portfolio-site-six-liart.vercel.app/api?username=YOUR_GITHUB_USERNAME&show_icons=true&theme=radical&count_private=true)](https://github.com/anuraghazra/github-readme-stats)
[![Top Langs](https://portfolio-site-six-liart.vercel.app/api/top-langs/?username=YOUR_GITHUB_USERNAME&layout=compact&theme=radical)](https://github.com/anuraghazra/github-readme-stats)

**Important:** Replace `YOUR_GITHUB_USERNAME` with your actual GitHub username in the links above!

**About the Stats:**

These cards dynamically display my GitHub statistics using [Anurag Hazra's GitHub Readme Stats](https://github.com/anuraghazra/github-readme-stats).  The cards are served from my Vercel deployment at `https://portfolio-site-six-liart.vercel.app/` for fast and reliable updates.  The stats are fetched directly from the GitHub API using a Personal Access Token (PAT) for accurate and up-to-date information, *including private contributions* because `count_private=true` is set.

**Breakdown of the Cards:**

*   **First Card (My GitHub Stats):** This card shows an overview of my GitHub activity, including:
    *   Total Stars Earned
    *   Total Commits (in the last year by default; see `include_all_commits` below to change this)
    *   Total Pull Requests
    *   Total Issues Opened
    *   Total Contributions (including private contributions because `count_private=true` is set)
    *   A rank based on my activity.
    *   Icons indicating my main contributions (commits, PRs, issues, etc.).

*   **Second Card (Top Langs):** This card displays the languages I use most frequently in my repositories. The size of each segment is proportional to the amount of code I've written in that language.  `layout=compact` makes it a smaller, more concise chart.

**Customization and Configuration (IMPORTANT):**

These cards are highly customizable!  You can modify the appearance and data displayed by changing the query parameters in the URLs. Here's a breakdown of the key options, including those used above, and *crucially*, how to show all-time commits and exclude repositories:

1.  **`username` (REQUIRED):**  This is your GitHub username.  **You MUST replace `YOUR_GITHUB_USERNAME` with your actual username.**

2.  **`show_icons` (Optional):**  `true` displays icons (as in the example). `false` hides them.

3.  **`theme` (Optional):**  Changes the color scheme. The example uses `radical`.  Many other themes are available:
    *   `default`
    *   `dark`
    *   `radical`
    *   `merko`
    *   `gruvbox`
    *   `tokyonight`
    *   `onedark`
    *   `cobalt`
    *   `synthwave`
    *   `highcontrast`
    *   `dracula`
    *   ...and many more! (See the [GitHub Readme Stats documentation](https://github.com/anuraghazra/github-readme-stats#themes)). You can even create custom themes.

4.  **`layout` (Top Langs Card Only):**
    *   `default`: The standard layout.
    *   `compact`: A smaller, condensed layout (used in the example).

5.  **`count_private` (VERY IMPORTANT - Already Set):**
    *   The example *already includes* `&count_private=true` in the first card's URL.  This means your private contributions are being counted.  This *requires* a Personal Access Token (PAT) with the `repo` scope (and `read:user` if you want to include private contributions).  You've confirmed your PAT is set up correctly.  If you *don't* want to count private contributions, remove this part of the URL.

6.  **`include_all_commits` (IMPORTANT for All-Time Commits):**
    *   By default, the commit count is for the *past year only*.  To show your *total* commits across *all* years, add `&include_all_commits=true` to the URL of the *first* stats card (the overall stats card, *not* Top Langs).
    *   Example (add this to the first card URL): `&include_all_commits=true`
    *   **Warning:**  This can be *significantly* slower, especially if you have many years of GitHub activity.

7.  **`hide` (Optional):**  Hide specific stats.  Example: `&hide=issues` (hides issues). Separate multiple stats with commas: `&hide=issues,prs`.

8.  **`hide_title` (Optional):**  `true` hides the card title.

9.  **`hide_border` (Optional):**  `true` hides the card border.

10. **`line_height` (Optional):** Adjust line height (e.g., `&line_height=30`).

11. **`title_color` (Optional):** Customize title color (hex code, e.g., `&title_color=FF0000` for red).

12. **`text_color` (Optional):** Customize text color.

13. **`icon_color` (Optional):** Customize icon color.

14. **`bg_color` (Optional):** Customize background color.

15. **`langs_count` (Top Langs Card Only - Optional):** Number of languages to display.  Example: `&langs_count=10` (shows top 10).

16. **`exclude_repo` (Top Langs Card Only - IMPORTANT):**  Exclude specific repositories from the Top Languages calculation.  *Essential* if you have repositories with generated code, test data, or forks that skew your language stats.  Provide a comma-separated list: `&exclude_repo=repo1,repo2,repo3`.

**Example with All Commits and Excluded Repositories:**

```markdown
[![My GitHub Stats](https://portfolio-site-six-liart.vercel.app/api?username=YOUR_GITHUB_USERNAME&show_icons=true&theme=dracula&count_private=true&include_all_commits=true)](https://github.com/anuraghazra/github-readme-stats)
[![Top Langs](https://portfolio-site-six-liart.vercel.app/api/top-langs/?username=YOUR_GITHUB_USERNAME&layout=compact&theme=dracula&exclude_repo=repo-to-exclude,another-repo-to-exclude)](https://github.com/anuraghazra/github-readme-stats)
