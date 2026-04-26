# RBR Racestat Browser

Desktop tool for analyzing Richard Burns Rally (RallySimFans) driving data.

## Features

* **Stage Times**

  * View all runs (time, car, stage, session)
  * Sorting and filtering

* **Statistics Overview**

  * Total runs, completion rate
  * Most used cars and stages

* **Analysis views**

  * **Stage Analysis** – performance per stage
  * **Car Analysis** – performance per car
  * **Session Analysis** – performance by session type (Practice / Hotlap / Race)

## Download

https://github.com/mkujala/rbr-racestat-browser-releases/releases/latest

## Requirements

* RBR RaceStat database:

  ```
  raceStatDB.sqlite3
  ```

  Located in:

  ```
  \Richard Burns Rally\Plugins\NGPCarMenu\RaceStat\
  ```

* On first launch, select the database manually.

## Key Concepts

* **Runs** = all attempts

* **Completed** = finished runs only

* **Completion %** = completed runs / all runs

* **Completed km**

  * Distance from completed runs only

* **Min runs**

  * Minimum sample size required for analysis

* **Avg gap (s/km)**

  * Time difference per kilometer vs. your fastest run with the same car

* **Avg gap filter (Top N)**

  * Uses only best runs (Top 5 / 10 / 20)
  * Reduces noise from bad runs

## Notes

* Read-only application (does not modify database)
* Runs fully locally (no network usage)
* Settings stored in: AppData/Roaming/racestat-go/

## Changelog

### v0.10.2 (beta)

* Minor UI polish (Statistics Overview dropdown alignment)
* Improved filtering logic:

  * Car ↔ Stage dependency (Stage Times & Analysis views)
* Stability improvements:

  * Dropdown lifecycle fixes
  * Reduced crash scenarios in Statistics

## Bug Reports

Report issues via GitHub Issues.

Include:

* App version
* Windows version
* Steps to reproduce
* Screenshots or logs (if available)

## Acknowledgements

* Thanks to Mika-N, developer of NGPCarMenu / RaceStatDB, for the database data this application analyzes.
* RaceStatDB is part of the NGPCarMenu plugin project

## Author of RBR Racestat Browser

MogFin
