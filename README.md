```mermaid
---
title: SCRB Matrix Organization
---
block
    columns 3
    block:test:3
        %%columns auto (default)
        man["Department Managers"]:3
        man_elec man_mech man_soft
    end
    space:3
    block:meme
        columns 1
        uct("test")
        man_elec_
        ma_elec_
        au_elec_
        dr_elec_
        mf_elec_
        pw_elec_
        tc_elec_
    end
    man_elec --> meme
class uct BT
classDef BT stroke:transparent,fill:transparent
```
