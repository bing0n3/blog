---
layout: article
title: "GsoC CHAOSS/Augur"
author: "bing0ne"
date: 2019-08-24T12:15:02+08:00
tags: ["GsoC"]
slug: "gsoc-final"
categories: ["GSoC"]
toc: false
---

## Work Done in the summer 

* Develop new ui frontend for Augur 
* Implement Risk Metrics and Evolution Metrics 
* Implement Augur Worker

<!--more-->

## Pull Requests Merged 

* [chaoss/augur#287](https://github.com/chaoss/augur/pull/287): Implement Evolution Metrics in Community Growth Area 
* [chaoss/augur#292](https://github.com/chaoss/augur/pull/292): refactor metrics and add routes
* [chaoss/augur#295](https://github.com/chaoss/augur/pull/295): add unit test for evolution metrics and implement helper functions in frontend
* [chaoss/Augur#297](https://github.com/chaoss/augur/pull/297): Initial repo_group_id and repo_id when Re
* [chaoss/Augur#299](https://github.com/chaoss/augur/pull/299):Implement evolution metrics and Optimize Chart
* [chaoss/Augur#301](https://github.com/chaoss/augur/pull/301): Optimize frontend to prevent duplicate requests
- [chaoss/Augur#307](https://github.com/chaoss/augur/pull/307): add visulization metrics for Issue Card to brunch dev
- [chaoss/Augur#311](https://github.com/chaoss/augur/pull/311): stable-demo: add visulization metrics for Issue Card
- [chaoss/Augur#317](https://github.com/chaoss/augur/pull/317): Dev: Refactored the following metric implementations to include 'repo_name' 
- [chaoss/Augur#319](https://github.com/chaoss/augur/pull/319): Dev: fix API test fail caused by issues_closed_resolution_duration
- [chaoss/Augur#322](https://github.com/chaoss/augur/pull/322): Implement Facade metrics in augur_db database 
- [bing0n3/Augur-frontend](https://github.com/bing0n3/augur-frontend): new frontend repo
- [chaoss/Augur#325](https://github.com/chaoss/augur/pull/325): Add Metric Status Worker and Translate Repo function in AugurAPI.ts
- [chaoss/Augur#329](https://github.com/chaoss/augur/pull/329): update doc installing-augur.md 
- [chaoss/Augur#331](https://github.com/chaoss/augur/pull/331): Implement Risk metrics and Translate Component in frontend #331
- [chaoss/Augur#332](https://github.com/chaoss/augur/pull/329): Persist Vuex State to local 
- [chaoss/Augur#335](https://github.com/chaoss/augur/pull/335): Add a new Vuex module 'compare' 
- [chaoss/Augur#338](https://github.com/chaoss/augur/pull/338): add CompareControl Component
- [chaoss/Augur#341](https://github.com/chaoss/augur/pull/341): Refactor Metric Status Worker
- [chaoss/Augur#347](https://github.com/chaoss/augur/pull/347): add repo group and progress bar when retrieve date
- [chaoss/Augur#345](https://github.com/chaoss/augur/pull/345): Frontend Router and Risk Metric Implemntation

## Future Work 

1. Insights click takes you somewhere to see context
2. Most recent insights displayed on dashboard
3. Comparison working and intuitive 
4. Tick chart for developers
5. Add issues information to the repos page: Issue line chart 
6. Put whatever was on the risk page back  (button styling) 
7. Insights for a repo on a repo page
8. Explore insights page organized by repo group, ranked by recency
9. Repo Group Summary Page
