---
title: "GsoC Week 8 Summary"
author: "bing0ne"
date: 2019-07-21T20:35:02+08:00
tags: ["GsoC"]
slug: "gsoc-week8"
categories: ["GSoC"]
---

This week is the 8th week of Google Summer of Week. I focused on moving frontend to a separate repo and converted javascript to typescript. 

<!--more-->

## Meeting Log

Date: N/A


## Work Done this Week

- Frontend
  - Translate Vue Component to class style component in Typescript
    - Repos.vue
    - RepoGroups.vue
    - Fix the problem Vuex's mapAction and mapGetter not work
  - Optimize AugurAPI.ts 
    - Translate `Repo()` function to class
    - Add a `RepoGroup()` class

- Backend 
  - Add Risk Metric Implementation 
    - CII Best Practice
    - Committers
    - License Declared
    - License Coverage
    - License Count
    - **Note**: unit test not added because of need data. 

- Document 
  - Test Drive Aguru Installation instruction 

### Work Still in Progress
- Load Data correctly when we access a page through a URL. 
  - Optimize `getRepoRelations()` method
- Translate RepoOverview.vue and move function to action or mutation

### Pull Requests
- [chaoss/Augur#329](https://github.com/chaoss/augur/pull/329): update doc installing-augur.md 
- [chaoss/Augur#331](https://github.com/chaoss/augur/pull/319): Implement Risk metrics and Translate Component in frontend #331
- [chaoss/Augur#325](https://github.com/chaoss/augur/pull/325): Add Metric Status Worker and Translate Repo function in AugurAPI.ts



## Challenges Encountered
- We changed Augur frontend stucture, and trun Vuex to leverage modules, take two days to learn how Vuex works in the new structure. And In the typescript, we should declare Vuex actions, getters and mutations in the class for call these functions. 
- `spdx` schema only have a few data and data is not consistent with `augur_data`

## Future Work 
- Persist Vuex state into cookie, and import a new package `vuex-persistedstate`
- Start to convert visulization chart
- More future plans for next week to be decided in the next meeting on Monday, 22th July 2019.
- Optimize metric_status worker