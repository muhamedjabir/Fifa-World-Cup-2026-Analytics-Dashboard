#  FIFA World Cup 2026 — Live Analytics Dashboard

 A real-time analytics dashboard tracking every match, goal, and stat of FIFA World Cup 2026 — built from scratch with HTML, CSS, and vanilla JavaScript. No frameworks. No paid APIs. Fully free.

 Its fully created through Claude AI by vibe code.

🔗 **Live Demo:** https://muhamedjabir.github.io/Fifa-World-Cup-2026-Analytics-Dashboard/


## Project Overview

The FIFA World Cup 2026 is the biggest tournament in football history — 48 teams, 104 matches, 3 host nations (USA, Canada, Mexico). As a data analyst, I wanted to go beyond just watching the matches and actually analyze the tournament as it unfolds.

This dashboard was built to answer real questions:

- Which team is performing best so far?
- Which matchday had the most goals?
- When in a match are most goals scored?
- Which groups are the most competitive?
- Who is leading the Golden Boot race?
- Which teams are on a winning streak?
- Which matches had the most dramatic comebacks?

Every answer updates automatically. No manual data entry. No refreshing spreadsheets. Just open the page — and the data is there.

## How Auto-Update Works


User opens dashboard
        ↓
Fetches latest JSON from openfootball GitHub (free, open-source)
        ↓
All stats, charts, standings recalculated instantly
        ↓
If fetch fails → loads embedded backup data + shows offline notice
        ↓
User clicks Refresh → retries live fetch

Data source updates within a few hours of each match finishing. Every page load = fresh data.


##  Dashboard Features

### Overview Tab

- Live tournament stats (matches played, total goals, goals/match, remaining fixtures)
- Last 5 results + next 5 upcoming fixtures
- Top 5 scorers snapshot
- Group A standings snapshot
- Most exciting matches ranked by total goals
- Clean sheet tracker

### Matches Tab

- All 104 matches sorted by date
- Filter by: All / Finished / Upcoming
- Search by team name — type "Brazil" → shows only Brazil matches
- Click any finished match → popup shows goalscorers, minute of each goal, HT score, venue
- All kickoff times in **Indian Standard Time (IST)**

### Standings Tab

- All 12 groups (A through L)
- Live W/D/L/GF/GA/GD/Points for every team
- Auto-calculated from match results
- Color-coded: Gold = qualified, Blue = 3rd place contender, Red = eliminated

### Top Scorers Tab

- Full Golden Boot leaderboard
- Goal bar showing relative scoring rate
- Updates after every matchday

### Charts Tab
- Goals per matchday bar chart (above/below average highlighted)
- Match outcome donut chart (Home Win / Draw / Away Win %)
- Top 10 teams by goals scored

### Analytics Tab
**This is the core data analyst section.**

**Tournament Summary Cards**

- Goals per match average
- Biggest win margin
- Highest scoring match
- Most goals in a single day
- Draw rate %
- Home nation win rate

**Tournament Pace Analysis:**

-  Bar chart showing goals per matchday
- Gold line = tournament average
- Instantly shows if tournament is getting more or less exciting over time

**Scoring Patterns:**

- Goals broken into 15-minute buckets (1–15, 16–30, 31–45, 46–60, 61–75, 76–90, 90+)
- 1st Half vs 2nd Half goal split with percentages
  

**Group Difficulty Score:**

- Custom formula: Goals/Match + (Draw Rate × 2) − Avg Margin × 0.3
- Ranks all 12 groups by competitiveness
- Answers: *Which group is the toughest?*

### Group Progress Tab

- All 12 groups with current qualification status
- Live W/D/L record per team
- "✓ Through" / "Eliminated" / "Top 2" badges

### Bracket Tab

- Knockout stage bracket
- Populates automatically as teams qualify from group stage
- Winners highlighted in gold

**Team Form Guide:**
- Last 3 match results per team → W/D/L badges
- Points from last 3 games — shows current momentum

**Goals For vs Goals Against:**
- Dual bar chart per team
- Attack strength vs defensive weakness at a glance

**Comeback Tracker:**
- Matches where a team was losing at HT → won or drew at FT
- Clickable → opens match detail popup

**Scoreless Half Analysis:**
- How many matches had 0 goals in 1st half vs 2nd half
- Auto-generated insight text

**Winning Margin Distribution:**
- 1 goal / 2 goals / 3 goals / 4+ goals / Draw
- Shows overall competitiveness of the tournament

**Insights:**
- Shows insights after every matches it will update automatically


Numbers update automatically with each page load



## Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Structure |
| CSS3 | Styling, animations, responsive design |
| Vanilla JavaScript | All logic, data processing, chart rendering |
| Canvas API | Donut chart rendering |
| Fetch API | Live data retrieval |
| openfootball/worldcup.json | Free open-source match data |
| GitHub Pages | Free hosting |

Zero paid tools. Zero frameworks. Zero backend.


## Error Handling

| Scenario | Behavior |
|---|---|
| No internet connection | Loads embedded backup + shows offline badge |
| GitHub API timeout (8s) | Falls back to backup + shows toast notification |
| Empty data returned | Catches error, loads backup |
| HTTP 4xx/5xx error | Shows exact error code in toast |
| User retries | Fresh fetch attempt via "Try again" button |

## 📱 Responsive Design

| Device | Breakpoint | Behavior |
|---|---|---|
| Desktop | 1400px max | Full layout, all columns visible |
| Tablet | < 1000px | 2-column grid collapses to 1 |
| Mobile | < 768px | Compact rows, scrollable tabs, venue column hidden |
| Small mobile | < 400px | Single column, minimal text, group badge hidden |


## Tournament Info

| Detail | Info |
|---|---|
| Start date | June 11, 2026 |
| Final | July 19, 2026 |
| Host nations | USA 🇺🇸 · Canada 🇨🇦 · Mexico 🇲🇽 |
| Teams | 48 (expanded from 32) |
| Total matches | 104 |
| Venues | 16 stadiums |
| Groups | 12 (A through L) |


## Data Source

Data from [openfootball/worldcup.json](https://github.com/openfootball/worldcup.json) — open public domain football data maintained by Gerald Bauer. Updates daily during the tournament.


## The Author

**Muhamed Jabir**
BCom Computer Application — Calicut University
Aspiring Data Analyst | Malappuram, Kerala

Building real-world analytics projects using SQL, Excel, Power BI, and Python.

- Portfolio: https://muhamedjabir.github.io/
- LinkedIn: https://www.linkedin.com/in/muhamed-jabir/

