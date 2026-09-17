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

    group projects[Projects]
    group au[Autonomy] in projects
        service elec_au[Electrical Arm Member] in au
        service mech_au[Mechanical Arm Member] in au
        service soft_au[Software Arm Member] in au
    group dr[Drone] in projects
        service elec_dr[Electrical Arm Member] in dr
        service mech_dr[Mechanical Arm Member] in dr
        service soft_dr[Software Arm Member] in dr
    group mf[Mobility & Frame] in projects
        service elec_mf[Electrical Arm Member] in mf
        service mech_mf[Mechanical Arm Member] in mf
        service soft_mf[Software Arm Member] in mf
    group pw[Power] in projects
        service elec_pw[Electrical Arm Member] in pw
        service mech_pw[Mechanical Arm Member] in pw
        service soft_pw[Software Arm Member] in pw
    group tc[TT&C] in projects
        service elec_tc[Electrical Arm Member] in tc
        service mech_tc[Mechanical Arm Member] in tc
        service soft_tc[Software Arm Member] in tc

    group ma[Arm] in projects
        service elec_ma[Electrical Arm Member] in ma
        service mech_ma[Mechanical Arm Member] in ma
        service soft_ma[Software Arm Member] in ma

    align row elec_ma mech_ma soft_ma
    align row elec_man mech_man soft_man
    align column ma_lead au_lead dr_lead mf_lead pw_lead tc_lead
    ma_lead:R --> L:elec_ma{group}
    

```
