```mermaid
---
title: SCRB Matrix Organization
---
architecture-beta
    group disciplines[Departments]
        service elec[Electrical] in disciplines
        service mech[Mechanical] in disciplines
        service soft[Software] in disciplines

    group projects[Projects]
        service arm[Arm] in projects
```
