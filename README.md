# 1D-arrays-creating
Ways to create one-dimensional arrays

Actual for NET 6.0

```C#
var a = (int[])Array.CreateInstance(typeof(int), 3); // { 0, 0, 0 }
var a = new int[3];               // { 0, 0, 0 }
var a = new int[3] { 1, 2, 3 };   // { 1, 2, 3 }
var a = new int[] { 1, 2, 3 };    // { 1, 2, 3 }
var a = new [] { 1, 2, 3 };       // { 1, 2, 3 }
int[] a = { 1, 2, 3};             // { 1, 2, 3 }
var a = Enumerable.Range(1, 3).ToArray(); // { 1, 2, 3 }


var a = new int[0];               // {  }
var a = Array.Empty<int>();       // {  }

var a = new[] { 1.0f, 2.0, 3 };         // only for double
double[] a = new[] { 1.0f, 2.0, 3 };    // only for double

object[] a = { "text", 1.0, 2 };
Console.WriteLine(a[0]); // text
Console.WriteLine(a[1]); // 1
Console.WriteLine(a[2]); // 2
```
