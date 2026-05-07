# UK Public Sector GitHub Repository Scraper

> **Fork note:** This is a fork of [uk-x-gov-software-community/xgov-opensource-repo-scraper](https://github.com/uk-x-gov-software-community/xgov-opensource-repo-scraper). The vast majority of the work was done by the original authors. Changes from the original:
> - Uses an updated list of UK public sector orgs from [chrishylanduk/government.github.com@add-uk-public-sector-orgs-202602](https://github.com/chrishylanduk/government.github.com/tree/add-uk-public-sector-orgs-202602)
> - Added a keepalive GitHub Action to stop the scraper being disabled automatically
> - Removed the web dashboard, SBOM scraping, and Google Sheets references — this fork just scrapes repos and publishes the JSON

[![Publisher](https://github.com/chrishylanduk/xgov-opensource-repo-scraper/actions/workflows/main.yml/badge.svg)](https://github.com/chrishylanduk/xgov-opensource-repo-scraper/actions/workflows/main.yml)

A tool that scrapes [UK public sector organisations on GitHub](https://government.github.com/community/) and records stats about their repositories, updated nightly via GitHub Actions.

## Data

The raw data is available as [repos.json](https://chrishylanduk.github.io/xgov-opensource-repo-scraper/repos.json).

You can also [explore the data with Datasette Lite](https://lite.datasette.io/?json=https://chrishylanduk.github.io/xgov-opensource-repo-scraper/repos.json#/data/repos) — loads the JSON into SQLite in your browser for full SQL querying with no server required.
