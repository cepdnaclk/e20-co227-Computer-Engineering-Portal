---
layout: home
permalink: index.html

repository-name: e20-co227-Computer-Engineering-Portal
title: Computer Engineering Portal
---

# Computer Engineering Portal

---

## Team
-  E/20/087: Supun Dulara, [e20087@eng.pdn.ac.lk](mailto:e20087@eng.pdn.ac.lk)
-  E/20/094: Ishara Ekanayaka, [e20094@eng.pdn.ac.lk](mailto:e20094@eng.pdn.ac.lk)
-  E/20/131: S.T.S Hasantha, [e20131@eng.pdn.ac.lk](mailto:e20131@eng.pdn.ac.lk)
-  E/20/179: Kusal Jayawardhana, [e20179@engdn.ac.lk](mailto:e20179@engdn.ac.lk)

## Table of Contents
1. [Introduction](#introduction)
2. [Content Management](#content-management)
3. [Course Management](#course-management)
4. [Taxonomy Integration](#taxonomy-integration)
5. [Links](#links)

---

## Introduction

The Computer Engineering Portal serves as both the internal and public web service platform for the Department of Computer Engineering, University of Peradeniya. This project includes content management(News and events),  course management and taxonomy integration.The portal is developed using Laravel framework and is deployed on [portal.ce.pdn.ac.lk](http://portal.ce.pdn.ac.lk).

## Content Management

News, Events, Seminars which are published on department website are managed through this portal. 

### News
- For the all news, visit: [portal.ce.pdn.ac.lk/api/news/v1](http://portal.ce.pdn.ac.lk/api/news/v1)
- Search by id: [portal.ce.pdn.ac.lk/api/news/v1/{id}](http://portal.ce.pdn.ac.lk/api/news/v1/{id})

### Events
- For all events, visit: [portal.ce.pdn.ac.lk/api/events/v1](http://portal.ce.pdn.ac.lk/api/events/v1)
- Upcoming events: [portal.ce.pdn.ac.lk/api/events/v1/upcoming](http://portal.ce.pdn.ac.lk/api/events/v1/upcoming)
- Past events: [portal.ce.pdn.ac.lk/api/events/v1/past](http://portal.ce.pdn.ac.lk/api/events/v1/past)
- Search by id: [portal.ce.pdn.ac.lk/api/events/v1/{id}](http://portal.ce.pdn.ac.lk/api/events/v1/{id})

## Content Management System

Course details are published on department website.This portal is used to manage the course details.Both undergraduate and postgraduate courses are managed through this portal.

- Undergraduate courses: [portal.ce.pdn.ac.lk/api/academic/v1/undergraduate/courses](http://portal.ce.pdn.ac.lk/api/academic/v1/undergraduate/courses)
- Undergraduate semesters: [portal.ce.pdn.ac.lk/api/academic/v1/undergraduate/semesters](http://portal.ce.pdn.ac.lk/api/academic/v1/undergraduate/semesters)

## Taxonomy Integration

This portal is used to manage taxonomies. Taxonomies are used to categorize various content.Here is some of the taxonomies used in this portal.

```
CEIntranet
├── For Students
│   ├── Academic Calendar
│   ├── Timetables
│   ├── Examination Schedules
│   ├── Academic Calendar
│   └── Advisor-Advisee
│
└── For Staff
    ├── Exam Claim Application
    ├── Examination Progress
    ├── Work Allocation
    └── Department Meeting Minutes
```

CEIntranet has property as Link. so every taxonomy term created in CEIntranet Should have a Link.

```
Students
├── Undergraduate Students
│   ├── E20
│   ├── E19
│   └── E18
│
├── Postgraduate Students
│
└── Alumni Students
    ├── E17
    ├── E16
    ├── E15
    ├── E14
    ├── E13
    ├── E12
    └── E11
```

Student taxonomy has these properties

- Academic Start Date: Date when the academic period begins
- Academic End Date: Date when the academic period ends
- Profiles Page: URL to the student profiles
- Notes: Additional information about the batch

So every taxonomy term created in Students Should have these properties.

## Links

- [Project Repository](https://github.com/cepdnaclk/{{ page.repository-name }}){:target="_blank"}
- [Project Page](https://cepdnaclk.github.io/{{ page.repository-name}}){:target="_blank"}
- [Department of Computer Engineering](http://www.ce.pdn.ac.lk/)
- [University of Peradeniya](https://eng.pdn.ac.lk/)