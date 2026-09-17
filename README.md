```mermaid
---
title: SCRB Matrix Organization
---
architecture-beta
    group disciplines[Departments]
        service elec[Electrical] in disciplines
        service mech[Mechanical] in disciplines
        service soft[Software] in disciplines

    group projects[Projects] in disciplines
        service ma()[Arm] in projects
        service au[Autonomy] in projects
        service dr[Drone] in projects
        service mf[Mobility & Frame] in projects
        service pw[Power] in projects
        service tc[TT&C] in projects 
    align row elec mech soft
    align column ma au dr mf pw tc
```
