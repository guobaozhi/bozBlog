---
Tags: # 标签数量丰俭由人
  - SQL
TocOpen: true
author:
  - boz
comments: true
cover:
  alt: ''
  caption: ''
  image: 'posts/cover.jpg'
  relative: true
date: '2025-03-14'
description: 'sql join commands' # 为页头简介，省略
hidesummary: false
disableShare: true
draft: false # 未发布时为 true
hidemeta: false
lastmod: '2025-03-14'
showToc: true
showbreadcrumbs: true
slug: ''
summary: 'list of SQL Joins commands'
title:  SQL Joins Cheatsheet
weight: null # 若置顶则为对应数字
---

# SQL Joins Cheatsheet
## LEFT JOIN
```sql
SELECT * FROM T1
LEFT JOIN T2
ON T1.NAME = T2.NAME
```

## INNER JOIN
```sql
SELECT * FROM T1
INNER JOIN
ON T1.NAME = T2.NAME
```

## RIGHT JOIN
```sql
SELECT * FROM T1
RIGHT JOIN
ON T1.NAME = T2.NAME
```

## LEFT JOIN (EXCLUDE T2)
```sql
SELECT * FROM T1
LEFT JOIN T2
ON T1.NAME = T2.NAME
WHERE T2.ID IS NULL
```

## UNION ALL (EXCLUDE INNER)
```sql
SELECT * FROM T1
LEFT JOIN ON T1.NAME = T2.NAME
WHERE T2.ID IS NULL
UNION ALL
SELECT * FROM T1
RIGHT JOIN T2 ON T1.NAME = T2.NAME
WHRE T1.ID IS NULL
```

## RIGHT JOIN  (EXCLUDE T1)
```sql
SELECT * FROM T1
RIGHT JOIN T2
ON T1.NAME = T2.NAME
WHERE T1.ID IS NULL
```

## FULL OUTER JOIN
```sql
SELECT * FROM T1
FULL OUTER JOIN T2
ON T1.NAME = T2.NAME
```

## UNION ALL
```sql
SELECT * FROM T1
LEFT JOIN T2 ON T1.NAME = T2.NAME
UNION ALL
SELECT * FROM T1
RIGHT JOIN T2 ON T1.NAME = T2.NAME
WHERE T1.ID IS NULL
```

link: sysxplore.com