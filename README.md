```mermaid
---
title: SCRB Matrix Organization
---
architecture-beta
    group managers[Department Managers]
        service elec_man[Electrical Manager] in managers
        service mech_man[Mechanical Manager] in managers
        service soft_man[Software Manager] in managers
    group leads[Project Leads]
        service ma_lead[Arm Lead] in leads
        service au_lead[Autonomy Lead] in leads
        service dr_lead[Drone Lead] in leads
        service mf_lead[Mobility & Frame Lead] in leads
        service pw_lead[Power Lead] in leads
        service tc_lead[TT&C Lead] in leads

    group elec_mem[Electrical Members]
        service temp[temp] in elec_mem

    group projects[Projects]
        service ma[Arm] in projects
        service au[Autonomy] in projects
        service dr[Drone] in projects
        service mf[Mobility & Frame] in projects
        service pw[Power] in projects
        service tc[TT&C] in projects
    align row elec mech soft
    align column ma au dr mf pw tc
    align column ma_lead au_lead dr_lead mf_lead pw_lead tc_lead
    ma_lead:R --> L:ma
    

```
