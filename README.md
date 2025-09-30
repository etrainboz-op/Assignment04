# Welcome to Assignment 04
This is my first GitHub pages project.

## Introduction paragraph
This page is made to show the difference between formatting integers, floats, and strings in languages Python and C.

## Integer Formatting

### C99 printf

'''c
#include <stdio.h>
int main()
{
    int n = 85;
    printf("%5d\n", n); // width 5, right-aligned
    printf("%+5d\n", n); // width 5, show sign
    printf("%05d\n", n); // width 5, pad with zeros
    return 0;
}

'''markdown
### Python print

'''python
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

