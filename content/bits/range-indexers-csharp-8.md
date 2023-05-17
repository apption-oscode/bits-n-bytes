---
title: "Range Indexers (C# 8.0+)"
date: 2023-05-17T16:14:06-04:00
draft: true
---

```csharp
var array = new int[] {​​​​​​​​​ 1, 2, 3, 4, 5 }​​​​​​​​​;
var slice1 = array[2..^3];  // array[new Range(2, new Index(3, fromEnd: true))]
var slice2 = array[..^3];   // array[Range.EndAt(new Index(3, fromEnd: true))]
var slice3 = array[2..];    // array[Range.StartAt(2)]
var slice4 = array[..];     // array[Range.All]
```