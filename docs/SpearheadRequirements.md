# Spearhead Battle Tracker — Requirements & User Stories

## Background: How Spearhead Scoring Works

Games are played over 4 rounds.

Each round has 2 turns (one for each player).

    In a round one player goes, then the other player goes.

    Players roll off and the winner decides if they are the attacker or defender.

    Defender picks the board layout, the attacker deploys their army first but gets to pick whether they take the first turn or not.

    At the start of the 2nd round and onward the players roll-off, the winner decides whether they want to take the first turn this round.

At the end of their turn, a player scores one victory point for holding an objective, another one for holding two or more objectives, one for holding more objectives than their opponent, and one for each "battle tactic" scored.

    Each player gets a deck of 12 cards, and at the start of each battle round draws three battle tactic cards. 
    Every card gives the choice between scoring a battle tactic or using a powerful command. 
    At the start of every battle round, the underdog — the person who is behind on victory points — draws a "twist card" that will impact the battle in some way, providing a bonus. 
    
The person with the most victory points is the winner. There is no tie-breaker, so games can end in a draw.

---

## Functional Requirements

### Player & Faction Management

| ID | Requirement |
|----|-------------|
| FR-01 | The system shall allow players to be created with a name |
| FR-02 | The system shall maintain a list of available Spearhead factions (e.g. Stormcast Eternals, Skaven, Sylvaneth) |
| FR-03 | A player shall be able to select which faction they played in a given match |

### Match Recording

| ID | Requirement |
|----|-------------|
| FR-04 | The system shall allow a new match to be recorded between two players |
| FR-05 | A match shall record the date it was played |
| FR-06 | A match shall record which faction each player used |
| FR-07 | A match shall record the victory point total for each player at the end of the game |
| FR-08 | A match shall record the victory points scored by each player per round (rounds 1–4) |
| FR-09 | A match shall record how many of each player's victory points came from objectives vs. battle tactics each round |
| FR-10 | A match shall record the result: Player 1 win, Player 2 win, or Draw |
| FR-11 | The result shall be automatically derived from the final Victory Point totals, not entered manually |
| FR-12 | A match shall record which battlefield (realm side) was used — Aqshy, Ghyran, Dolorum or Ossia |

### Statistics & History

| ID | Requirement |
|----|-------------|
| FR-13 | The system shall display a match history list showing all recorded games |
| FR-14 | The system shall display a win/loss/draw record between two players |
| FR-15 | The system shall display each player's overall win rate as a percentage |
| FR-16 | The system shall display the average total Victory Points scored per game, per player |
| FR-17 | The system shall display the average Victory Points scored per round, per player |
| FR-18 | The system shall display each player's win rate broken down by faction played as |
| FR-19 | The system shall display each player's win rate broken down by faction played against |
| FR-20 | The system shall display the highest Victory Points score ever recorded in a single game |

---

## User Stories

### Epic 1 — Player Setup

**US-01**
> As a player, I want to add myself and my brother-in-law as named players, so that the app knows who is playing.

**US-02**
> As a player, I want to select a faction from a list when recording a match, so that I don't have to type faction names manually.

---

### Epic 2 — Recording a Match

**US-03**
> As a player, I want to start a new match record and choose which two players are playing, so that the match is correctly attributed.

**US-04**
> As a player, I want to select which faction each player is using for this match, so that faction-level stats can be tracked.

**US-05**
> As a player, I want to enter how many Victory Points each player scored at the end of each round, so that the per-round breakdown is captured.

**US-06**
> As a player, I want to enter how many of each round's Victory Points came from objectives and how many came from battle tactics, so that I can see which scoring method we relied on most.

**US-07**
> As a player, I want the app to automatically determine the winner from the final Victory Points totals, so that I don't have to enter the result separately and can't enter it incorrectly.

**US-08**
> As a player, I want to record which realm side (Aqshy or Ghyran) was used, so that I can spot if one battlefield favours a particular player or faction.

**US-09**
> As a player, I want the match date to default to today, so that I don't have to enter it manually after every game.

---

### Epic 3 — Viewing History

**US-10**
> As a player, I want to see a list of all past matches showing the date, factions, and final score, so that I can review our battle history.

**US-11**
> As a player, I want to tap on a past match to see the full round-by-round breakdown, so that I can remember how the game unfolded.

---

### Epic 4 — Statistics

**US-12**
> As a player, I want to see my overall win/loss/draw record against my brother-in-law, so that I know who is winning our rivalry.

**US-13**
> As a player, I want to see each player's win rate as a percentage, so that the record is easy to read at a glance.

**US-14**
> As a player, I want to see my average Victory Points per game and per round, so that I can see if my scoring is improving over time.

**US-15**
> As a player, I want to see which faction I win most often with, so that I know my strongest army.

**US-16**
> As a player, I want to see which faction I struggle against most, so that I know where I need to improve.

**US-17**
> As a player, I want to see the highest Victory Points score ever recorded in a single game, so that we have a record to try and beat.

