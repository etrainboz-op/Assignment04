# Welcome to Assignment 04
This is my first GitHub pages project.

## Introduction paragraph
This page is made to show the difference between formatting integers, floats, and strings in languages Python and C.

## Integer Formatting

### C99 printf

<pre> 
```c
#include <stdio.h>
int main()
{
    int n = 85;
    printf("%5d\n", n); // width 5, right-aligned
    printf("%+5d\n", n); // width 5, show sign
    printf("%05d\n", n); // width 5, pad with zeros
    return 0;
}
```
</pre>

### Python print

<pre>
```python
// Old-style
n = 85
print("%5d" % n) # width 5, right-aligned
print("%+5d" % n) # width 5, show sign
print("%05d" % n) # width 5, pad with zeros

// F-strings
n = 85
print(f"{n:5}") # width 5, right-aligned
print(f"{n:+5}") # width 5, show sign
print(f"{n:05}") # width 5, pad with zeros
```
</pre>

## Float Formatting

### C99 printf

<pre> 
```c
#include <stdio.h>
int main()
{
    float f = 7.25743;
    printf("%8.2f\n", f); // width 8, 2 decimals
    printf("%08.2\n", f); // pad with zeros
    printf("%e\n", f); // scientific notation
    return 0;
}
```
</pre>

### Python print

<pre>
```python
// Old-style
f = 7.25743
print("%8.2f" % f) # width 8, 2 decimals
print("%08.2f" % f) # pad with zeros
print("%e" % f) # scientific notation

// F-strings
f = 7.25743
print(f"{f:8.2f}") # width 8, 2 decimals
print(f"{f:08.2f}") # pad with zeros
print(f"{f:e}") # scientific notation
```
</pre>

## String Formatting

### C99 printf

<pre> 
```c
#include <stdio.h>
int main()
{
    char *s = "Hello";
    printf(%-10s!\n", s); // left-aligned, width 10
    printf(%10s!\n", s); // right-aligned, width 10
    return 0;
}
```
</pre>

### Python print

<pre>
```python
// Old-style
s = "Hello"
print("%-10s!" % s) # left-aligned, width 10
print("%10s!" % s) # right-aligned, width 10

// F-strings
s = "Hello"
print(f"{s:<10}!") # left-aligned
print(f"{s:>10}!") # right-aligned
print(f"{s:^10}!") # centered
```
</pre>"