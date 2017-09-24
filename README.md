# Premier-League-Scraper
Match data for all the seasons in the English Premier League

### JSON Dump
JSON Dump Files contain detailed information about available matches. For some matches, this dump is unavailable on the official Premier League website. The stats file lists the erroneous data.

### Match Data
Match Data in following format :

| Season   | GW | MID | Date                | HID | Home    | AID | Away         | HT Home | HT Away | FT Home | FT Away | Referee   | Stadium  | City   | Attendance |
|----------|----|-----|---------------------|-----|---------|-----|--------------|---------|---------|---------|---------|-----------|----------|--------|------------|
| 11992-93 | 1  | 1   | 1992-08-15 15:00:00 | 1   | Arsenal | 14  | Norwich City | 2       | 0       | 2       | 4       | Alan Gunn | Highbury | London | 24030      |

##### Keywords 
1. GW - Gameweek
2. MID - Match ID (https://premierleague.com/match/[matchid])
3. HID - Home Team ID (https://premierleague.com/clubs/[teamid])
4. AID - Away Team ID
5. HT - Half Time
6. FT - Full Time

##### **Missing Data :** Attendance data not available for some matches. Nan values present instead.