# Uninitialized Property Access in C#

This repository demonstrates a common error in C#: accessing a property of a class before it has been assigned a value.  This can lead to unexpected results, typically the default value for the property's type (0 for integers, null for strings, etc.). The solution shows how to properly initialize the property to avoid this issue.

## Bug

The `bug.cs` file contains code that attempts to access the `MyProperty` of the `ExampleClass` before assigning a value. This results in the default value (0) being printed. 

## Solution

The `bugSolution.cs` file demonstrates the corrected code. The `MyProperty` is initialized in the constructor, ensuring it has a defined value when accessed in `MyMethod()`.