# Premier-League-Scraper
Match data for all the seasons in the English Premier League

### JSON Dump
JSON Dump Files contain detailed information about available matches. For some matches, this dump is unavailable on the official Premier League website. The stats file lists the erroneous data.

### Match Data
Match Data in following format :

| Season  | GW | MID | Date                | HID | Home    | AID | Away         | HT Home | HT Away | FT Home | FT Away | Referee   | Stadium  | City   | Attendance |
|---------|----|-----|---------------------|-----|---------|-----|--------------|---------|---------|---------|---------|-----------|----------|--------|------------|
| 1992-93 | 1  | 1   | 1992-08-15 15:00:00 | 1   | Arsenal | 14  | Norwich City | 2       | 0       | 2       | 4       | Alan Gunn | Highbury | London | 24030      |

##### Keywords 
1. GW - Gameweek
2. MID - Match ID (https://www.premierleague.com/match/[matchid])
3. HID - Home Team ID (https://www.premierleague.com/clubs/[teamid])
4. AID - Away Team ID
5. HT - Half Time
6. FT - Full Time

##### **Missing Data :** Attendance data not available for some matches. Nan values present instead.

### Event Data
Contains event by event information for all the matches. Available in following format :

| Season  | GW | MID | Home    | Away         | Minute | Event | PID | Player      | TID | Team    | AID | Assister         |
|---------|----|-----|---------|--------------|--------|-------|-----|-------------|-----|---------|-----|------------------|
| 1992-93 | 1  | 1   | Arsenal | Norwich City | 28'00  | G     | 9   | Steve Bould | 1   | Arsenal | 11  | Nigel Winterburn |

##### Keywords
1. PID - Player ID (https://www.premierleague.com/players/[playerid])
2. AID - Assister ID

##### Event Keywords
1. G - Goal
2. Y - Yellow Card
3. R - Red Card
4. YR - Second Yellow Card (Red Card)
5. P - Penalty
6. O - Own Goal
7. ON - Substitution On
8. OFF - Substitution Off

**Unknown/Missing Events** : 3 null events; 'SP', 'MP' events not visible on website but found in scraped data.