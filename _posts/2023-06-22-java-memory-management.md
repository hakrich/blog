---
title: "Java Memory Management"
date: 2023-06-22
---
Java applications are only allowed to use a limited amount of memory. This limit is specified during application startup. To make things more complex, Java memory is separated into two different regions. These regions are called Heap space and PermGen (for Permanent Generation, which is replaced by MetaSpace from Java8):

Heap space stores all objects created by your Java program. Its content is monitored by the garbage collector, which frees memory from the heap if you stop using the object (i.e. no more reference to the object)

Credited to: https://plumbr.io/outofmemoryerror/java-heap-space