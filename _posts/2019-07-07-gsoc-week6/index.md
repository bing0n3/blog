---
layout: article
title: "GsoC Week 6 Summary"
author: "bing0ne"
date: 2019-07-07T15:31:02+08:00
tags: ["GsoC"]
slug: "gsoc-week6"
categories: ["GSoC"]
---

This week is the 6th week of Google Summer of Week. I focused on moving frontend to a separate repo and converted javascript to typescript. 

<!--more-->

## Meeting Log

Date: 07/06/2019 

- Develop a script to pull metrics into `chass_metric_status table`

## Work Done this Week

- Metric Implementation 
  - annual-commit-count-ranked-by-new-repo-in-repo-group
  - annual-commit-count-ranked-by-repo-in-repo-group
  - annual-lines-of-code-count-ranked-by-repo-in-repo-group
  - annual-lines-of-code-count-ranked-by-new-repo-in-repo-group

- Move Frontend to new repo based on Vue-CLI 
  - converted `AugurAPI.js`, `Augur.js` and `AugurStats.js` to Tyepescript 

- Metrics Refactored
  - Refactor all metric API endpoints to include a repo-name field.

### Pull Requests
- [chaoss/Augur#317](https://github.com/chaoss/augur/pull/317): Dev: Refactored the following metric implementations to include 'repo_name' 
- [chaoss/Augur#319](https://github.com/chaoss/augur/pull/319): Dev: fix API test fail caused by issues_closed_resolution_duration
- [chaoss/Augur#322](https://github.com/chaoss/augur/pull/322): Implement Facade metrics in augur_db database 
- [bing0n3/Augur-frontend](https://github.com/bing0n3/augur-frontend): new frontend repo


## Challenges Encountered
* How to convert `js` to `ts`. And typescript is a new technique for me.
* Let `Vue-Cli` complie css correctly. 

## Future Work 
- Add script to pull `metirc` from chass metric repo. 
- More future plans for next week to be decided in the next meeting on Monday, 8th July 2019.


