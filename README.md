# Lacrosse Opponent Scouting

Opponent scouting and post-game dashboards built for UVA Women's Lacrosse in the 2026 season.

The goal was simple: turn game film and public box scores into a plan the coaching staff could use in the week before a game. That means showing where an opponent is predictable, where their goalkeeper is beatable, who runs their offence, and where their draws go.

## What is here

The four JMU dashboards. Each is a single HTML file, so you can download it and open it in any browser.

| Dashboard | What it covers |
|---|---|
| `dashboards/JMU_Offense_Scouting_Dashboard.html` | 17 offensive clips: formations, named plays, shot outcomes, transition, and a counter-plan for our defence |
| `dashboards/JMU_Defense_Scouting_Dashboard.html` | 14 defensive possessions: where their zone breaks (motion into a drive or cut, transition, man-down rotation) and how to attack it |
| `dashboards/JMU_GK_Scouting_Dashboard.html` | 109 shots against JMU over 5 games: shot origin, placement on the cage, save rate by zone and situation |
| `dashboards/JMU_Draw_Control_Scouting_Dashboard.html` | 32 draw controls: who takes them, where the ball goes, technique and wing play |

## How it was built

1. **Tagging.** Every shot, draw and possession clip was coded on a fixed set of fields: location, cage zone, shot type, situation (even, man-up, free position), technique and outcome.
2. **Models.** Zone-based expected goals and goals saved above expected for the goalkeeper, a weighted pre-game win-probability model with swing factors, and win probability added for the post-game review.
3. **Delivery.** Interactive dashboards (Chart.js and D3) with filters by game, player and situation. Each one ends with a game plan.

No tracking data was used. Everything comes from film, box scores and official play-by-play.

## Notes

The Pittsburgh scouting set and the UVA goalkeeper self-scout from the same season are not included here.

Code is MIT-licensed. Game film and team data belong to their owners.
