---
title: 'DAX新建表'
date: 2022-03-12 23:13:06
tags: [PowerBI,DAX]
published: true
hideInList: false
feature: 
isTop: false
---
Dax.新建表UnitTable = 
SELECTCOLUMNS(    //选择某张表，按上表头
    
//以下是新建表，但没有表头
    {
        ("K",1000),
        ("w",10000),
        ("M",1000000)
    },
//新建表

//按上表头
    "UnitName",[Value1],
    "UnitValue",[Value2]

)*