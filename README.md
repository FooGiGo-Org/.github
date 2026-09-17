```mermaid
---
title: SCRB Matrix Organization
---
graph TD;
  PM[Project Manager]
  SL[Systems Lead]
  subgraph Disciplines
    elec[Electrical Members]
    mech[Mechanical Members]
    soft[Software Members]
  end
  subgraph Project Leads
    ma_l[Arm Lead]
    au_l[Autonomy Lead]
    dr_l[Drone Lead]
    mf_l[Mobility & Frame Lead]
    pw_l[Power Lead]
    sp_l[Science Payload Lead]
    tc_l[TT&C Lead]
  end
  subgraphs Projects
    ma[Arm Project]
    au[Autonomy Project]
    dr[Drone Project]
    mf[Mobility & Frame Project]
    pw[Power Project]
    sp[Science Payload Project]
    tc[TT&C Project]
  end
```
