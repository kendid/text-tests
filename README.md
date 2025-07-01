# text-tests

```mermaid
  info
```

## Mermaid diagram?

```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title       Adding GANTT diagram functionality to mermaid
    excludes    weekends
    %% (`excludes` accepts specific dates in YYYY-MM-DD format, days of the week ("sunday") or "weekends", but not the word "weekdays".)

    section A section
    Completed task            :done,    des1, 2014-01-06,2014-01-08
    Active task               :active,  des2, 2014-01-09, 3d
    Future task               :         des3, after des2, 5d
    Future task2              :         des4, after des3, 5d

    section Critical tasks
    Completed task in the critical line :crit, done, 2014-01-06,24h
    Implement parser and jison          :crit, done, after des1, 2d
    Create tests for parser             :crit, active, 3d
    Future task in critical line        :crit, 5d
    Create tests for renderer           :2d
    Add to mermaid                      :until isadded
    Functionality added                 :milestone, isadded, 2014-01-25, 0d

    section Documentation
    Describe gantt syntax               :active, a1, after des1, 3d
    Add gantt diagram to demo page      :after a1  , 20h
    Add another diagram to demo page    :doc1, after a1  , 48h

    section Last section
    Describe gantt syntax               :after doc1, 3d
    Add gantt diagram to demo page      :20h
    Add another diagram to demo page    :48h
```

## Mermaid 2

```mermaid
flowchart LR
    FUK(福岡) --- YGT(山口)
    SAG(佐賀) --- FUK
    NGS() --- SAG
    FUK --- KMT(熊本)
    SAG --- KMT
    KMT --- ASO(麻生)
    ASO --- TCH(高千穂)
    TCH --- MYZ(宮崎)
    KMT --- KGS(鹿児島)
    KGS --- YKS(屋久島)
    KGS --- MYZ
    FUK --- YKS
    OKN(沖縄) --- FUK
    OKN --- KMT
    OKN --- KGS
    OKN --- MYZ
    ISG(石垣) --- FUK
    ISG --- OKN
    style KMT color:#aaa
    style KGS color:#aaa
    style MYZ color:#aaa
```
