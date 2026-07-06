# Türkiye Fired More Shots Than Anyone at the 2026 World Cup. So Why Did We Go Home?

*A data analysis of Turkey's group stage elimination — and what the numbers actually say about what went wrong.*

---

I watched all three of Turkey's group stage games this summer. After the Paraguay loss I was angry. After the Australia loss I was confused. By the time we beat the USA 3-2 in a dead rubber — after we were already eliminated — I wasn't even happy. Just empty.

The frustrating thing wasn't that we lost. It was *how* we lost. We had the ball. We had chances. We had Arda Güler pulling strings, Orkun Kökcü controlling the tempo, Baris Alper Yilmaz terrorizing fullbacks. We looked like a team that should be winning football matches. And yet, we weren't.

So I did what any data-obsessed fan does after a painful tournament exit: I opened a Jupyter notebook and started pulling numbers.

What I found surprised me — and honestly, made the elimination hurt even more.

---

## The Shot Problem Nobody Talked About

Let me start with the stat that should have been the headline of every Turkish football discussion this summer.

**Türkiye took 71 shots across three group stage games.**

That is the second most of any team in the entire tournament — only Belgium took more (73), and Belgium scored 5 goals doing it. More than France, who scored 10 goals. More than Argentina. More than Germany. 71 shots. In three games. Against Australia, Paraguay, and the United States.

We scored 3 goals. All of them against the USA, in a match that meant nothing for our qualification.

The immediate reaction is to blame bad luck. Posts, crossbars, world-class saves. And yes, some of that happened. But when you take 71 shots and score 3 goals, you stop looking for excuses and start looking for patterns.

The pattern is in the shot accuracy numbers.

**Turkey's Shot on Target percentage was 22.5%.** That means roughly 3 out of every 4 shots we took didn't even test the goalkeeper. Didn't hit the frame. Just sailed wide, clipped a defender, or ballooned over the bar. Among all 48 group-stage teams, that ranked us 5th from the bottom.

The Goals per Shot figure is even starker: **0.04**. For every 25 shots Turkey took, we scored once. The group stage average was roughly 0.12 — three times better than us.

This wasn't a finishing problem in the narrow sense. This was a shot quality problem. Turkey was shooting a lot, but shooting badly — from difficult angles, under pressure, from distance, in situations where the probability of scoring was always low. The volume masked the inefficiency.

---

## The Possession Paradox

Here's where it gets more complicated.

Turkey averaged **66.3% possession** across three games. That is the second highest figure in the entire group stage, behind only Spain. We had the ball more than almost anyone. We recycled it, we moved it, we pressed high to win it back when we lost it.

In theory, high possession leads to more chances, which leads to more goals. The data across the tournament shows a loose positive correlation — teams that controlled the ball tended to score more. Turkey was the glaring exception.

We had the ball constantly and converted almost none of it into goals. The possession didn't hurt us, but it didn't help us either. We turned it into a comfort blanket rather than a weapon. Lots of sideways passes in midfield. Lots of recycling. Not enough direct, purposeful movement into the areas that actually produce goals.

There's a concept in football analytics called **"positive possession"** — possession that actually progresses the ball toward danger. Turkey had plenty of the other kind.

---

## The xG Story: Worst Underperformance in the Tournament

xG, or Expected Goals, is the metric that cuts through both of those problems at once. It doesn't care how many shots you took or how much of the ball you had — it measures the *quality* of the chances you created, and asks: based on where these shots came from, how many goals should a team have scored?

For Turkey, across all three group stage games, the answer was **6.6 xG**.

We scored 3 goals.

That's a delta of **−3.6** — we underperformed our expected goals by 3.6 goals. I ran this against all 48 teams in the tournament.

Turkey's xG underperformance was the worst of any team in the entire 2026 World Cup. Not just among eliminated teams. Every team. 48 nations. Dead last.

For context: we created enough high-quality chances to have scored 6 or 7 goals in three games. A team that scores 6-7 goals in a World Cup group stage almost always advances. We created those chances and converted them at roughly half the expected rate.

The game-by-game breakdown tells the story even more starkly:

- **vs Australia (L 0-2):** 30 shots, 1.36 xG. We created decent chances and scored none. Australia created fewer and scored twice.
- **vs Paraguay (L 0-1):** 32 shots, 2.17 xG. Paraguay had 10 men for large parts of the match. We created the equivalent of two goals worth of chances with a numerical advantage. We scored none. They scored once from 7 shots.
- **vs USA (W 3-2):** 9 shots, 3.05 xG. We finally converted — and notably, with far fewer shots than the previous two games. Three goals from 9 attempts (0.34 xG per shot on average) shows what Turkey looked like when they actually shot from the right positions. Elimination already confirmed.

The pattern is consistent. It's not one bad game. Across all three matches, Turkey created quality chances and didn't put them away. That consistency is what separates a rough night from a systemic issue.

---

## The Defensive Side: Conceding Early, Conceding Often

The attack gets all the attention, but the defense wasn't innocent either.

Turkey conceded **5 goals** in three games, above the group stage average of 4.0. But the timing of those goals is what really hurt us.

Against Australia, we conceded in the 27th minute and never recovered — spending the rest of the game chasing the game with 70%+ possession and nothing to show for it. Against Paraguay, we conceded in the **2nd minute**. Two minutes. Before we'd even settled into the game. That goal forced us into exactly the kind of frantic, high-volume, low-quality attacking that the shot map captures.

There's a feedback loop here that the raw numbers don't fully show: early goals forced us into desperation possession, desperation possession produced low-quality shots, low-quality shots produced the worst xG conversion rate in the tournament. The defensive vulnerability upstream created the attacking inefficiency downstream.

Our opponents were also ruthlessly clinical. Australia scored 2 from 9 shots. Paraguay scored 1 from 7 shots with 10 men. They didn't need much — because they knew we'd give them the ball back, and they just needed to be dangerous on the counter.

---

## What the Data Suggests Needs to Change

I want to be careful here. Data can tell you *what* happened. It can't always tell you *why*, and it definitely can't pick a starting eleven or design a training session. But there are things the numbers strongly imply.

**Shot selection over shot volume.** 71 shots is not a badge of honor when 77% of them miss the target. The shot map shows a large proportion of Turkey's attempts coming from outside the box or from wide angles — positions where even a world-class finisher would struggle. The tactical priority should shift toward building play that ends in central box entries, not toward generating shot numbers.

**Converting the transition moments.** The games against Australia and Paraguay show that Turkey consistently had the better of possession and the better of chance creation. What we didn't do was score when opponents were disorganized. Quick transitions, direct play in the final third on the break — these situations produced Turkey's highest xG chances and the ones that got away.

**Defensive organization in the opening period.** Conceding in the 2nd and 27th minutes of two separate games isn't a coincidence. There's a structural issue in how Turkey set up in the early stages — possibly a high defensive line that left space in behind on early balls, possibly a pressing system that left gaps during transitions. Fixing this doesn't require a new striker. It requires a different approach to the first 30 minutes.

**The finishing question is complicated.** Yes, the xG delta of −3.6 implies finishing underperformance. But it's worth noting that over a three-game sample, variance is real. A post here, a great save there, and the number looks very different. The more structural problem is shot quality — and shot quality is determined by the system that generates chances, not just by the player who takes the final touch.

---

## Why This Matters Beyond One Tournament

Turkey came into this World Cup with arguably the best generation of attacking talent in decades. Arda Güler at Real Madrid. Kenan Yildiz at Juventus. Baris Alper Yilmaz operating at a high level for Galatasaray. The individual quality is not in question.

What the data reveals is a **system problem**, not a talent problem. We had the players to compete. We didn't have the structure to translate their quality into goals, or the defensive solidity to stay in games long enough for that quality to show up.

That's actually an optimistic finding, if you're willing to look at it that way. Talent is hard to develop. Systems can be changed. The raw material is there. The coaching staff, the tactical setup, the game model — those are the variables the numbers suggest need to evolve.

This generation of Turkish players won't be around forever. Güler is 19. Yildiz is 20. The window isn't closed. But if the 2026 World Cup taught us anything, it's that individual brilliance without systemic support produces exactly what we saw: beautiful possession, 71 shots, and an early flight home.

The data doesn't lie. Hopefully, those in charge of Turkish football are listening to it.

---

## A Note on the Data: How This Was Actually Built

Since this is also a portfolio project, I want to be transparent about the data acquisition process — because it didn't go according to plan, and the workaround is worth explaining.

**The plan:** use `soccerdata`, a Python library that wraps FBref scraping, to pull squad stats automatically. Clean, reproducible, two lines of code.

**What actually happened:** FBref blocks automated scraping. When `soccerdata` tried to fetch the squad stats pages, FBref returned a CAPTCHA challenge instead of data. When I tried `pandas.read_html()` directly, I got HTTP 403 Forbidden. FBref's data has commercial value — they sell it to clubs and broadcasters — so they actively defend against automated access.

This is a common and underappreciated problem in sports data analysis. The data exists, it's publicly visible in a browser, but programmatic access is blocked.

**The workaround:** I used a Chrome browser extension to read the page text from FBref as a real authenticated browser session, bypassing the scraping blocks entirely. The data was then hardcoded into the notebook as DataFrames — which for a completed, static tournament is actually the correct approach. The group stage is over, the numbers won't change, and hardcoded data is transparent and reproducible without network dependencies.

Note: eight teams (Germany, Netherlands, Brazil, Morocco, Japan, Canada, South Africa, Paraguay) had already advanced to the knockout rounds when the FBref data was first fetched, so their group-stage shooting stats were prorated from cumulative FBref figures using the formula: group_stage_shots = total_shots × (3 / total_90s_played).

For the per-match xG and shot data, I used FotMob (which sources from Opta), again read through the browser extension, since FotMob has no public API.

**The technical stack:**
- **Python + Jupyter Notebook** — analysis environment
- **pandas** — data manipulation and DataFrame construction
- **matplotlib + numpy** — all charts and visualizations
- **mplsoccer** — football pitch visualizations for the shot map
- **Data sources:** FBref (squad/shooting stats), FotMob/Opta (per-match xG, shot counts, possession), xGscore.io (full 48-team xG table)

**What I'd do differently with a budget:** Sportmonks or Opta APIs would provide structured, per-shot coordinate data — making the shot map pixel-precise rather than zone-approximated. StatsBomb's open data is also worth exploring for historical competitions they've chosen to release.

The full notebook and data are available on [GitHub](https://github.com/cbenli/turkey-football-analysis). The repo includes the `.gitignore` setup that excludes generated chart PNGs and Jupyter checkpoints — only the source notebook is versioned.

---

*All data sourced from FBref.com (squad/shooting stats) and FotMob/Opta (per-match xG, shot counts, possession), xGscore.io (full 48-team xG table). Analysis and visualizations produced in Python using pandas, matplotlib, and mplsoccer.*
