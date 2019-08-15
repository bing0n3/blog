---
title: "GsoC Week 11 Summary"
author: "bing0ne"
date: 2019-08-11T12:15:02+08:00
tags: ["GsoC"]
slug: "gsoc-week11"
categories: ["GSoC"]
---

This week is the 11th week of Google Summer of Week and the last week of third phase. 

<!--more-->

## Meeting Log

Date: 08/08/2019

- Implement Risk Metrics
- Add new visulization for risk metrics


## Work Done this Week

- Front End
  - fix style error 
    ![image](https://user-images.githubusercontent.com/15957393/62835633-4a089d80-bc8d-11e9-895f-7efc946b06c4.png)
  - Use repo_name instead url in the router 
  - Router for Repo comparison 
  - Add four visualization of risk metrics 
    ![205251565616838_ pic_hd](https://user-images.githubusercontent.com/15957393/62869452-77675100-bd4a-11e9-8149-ba2e11a42514.jpg)
    ![image](https://user-images.githubusercontent.com/15957393/62873538-2eb39600-bd52-11e9-8d08-32f62abcec92.png)

- Risk Metric 
  - refactor license-count
  - refactor license-coverage
  - refactor license-declared 
  - add test for all endpoints in risk metric 




### Pull Requests
- [chaoss/Augur#345](https://github.com/chaoss/augur/pull/345): Frontend Router and Risk Metric Implemntation 

## Challenges Encountered


## Future Work 
- Add new component for Repo Group 
- Convert more chart component into new version, for example `DynamicLineChart`