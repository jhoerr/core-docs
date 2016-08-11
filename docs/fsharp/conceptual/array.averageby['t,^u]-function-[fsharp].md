---
title: Array.averageBy<'T,^U> Function (F#)
description: Array.averageBy<'T,^U> Function (F#)
keywords: visual f#, f#, functional programming
author: dend
manager: danielfe
ms.date: 05/16/2016
ms.topic: language-reference
ms.prod: visual-studio-dev14
ms.technology: devlang-fsharp
ms.assetid: 9692ce07-61f4-4b49-adfb-618f9bd8f9c1 
---

# Array.averageBy<'T,^U> Function (F#)

Returns the average of the elements generated by applying the function to each element of the array.

**Namespace/Module Path:** Microsoft.FSharp.Collections.Array

**Assembly:** FSharp.Core (in FSharp.Core.dll)


## Syntax

```fsharp
// Signature:
Array.averageBy : ('T -> ^U) -> 'T [] -> ^U (requires ^U with static member (+) and ^U with static member DivideByInt and ^U with static member Zero)

// Usage:
Array.averageBy projection array
```

#### Parameters
*projection*
Type: **'T -&gt; ^U**


The function to transform the array elements before averaging.

*array*
Type: **'T**[[]](https://msdn.microsoft.com/library/def20292-9aae-4596-9275-b94e594f8493)

The input array.

## Exceptions
|Exception|Condition|
|---------|---------|
|[ArgumentException](https://msdn.microsoft.com/library/system.argumentexception.aspx)|Thrown when array is empty.|

## Return Value
The computed average.

## Remarks
This function is named `AverageBy` in compiled assemblies. If you are accessing the function from a language other than F#, or through reflection, use this name.

## Example

The following example illustrates the use of `Array.averageBy`.

[!code-fsharp[Main](../../../samples/snippets/fsarrays/snippet29.fs)]

**Output**

```
5.500000
```

## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2

## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable

## See Also
[Collections.Array Module &#40;F&#35;&#41;](Collections.Array-Module-%5BFSharp%5D.md)

[Microsoft.FSharp.Collections Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Collections-Namespace-%5BFSharp%5D.md)