# FlagsValues
Helper class that lists all valid values that an int-backed bit field enumeration type can have.

It can be used to help make sure that all members of an enumeration type are assigned valid values - powers of two between zero and [int.MaxValue](https://learn.microsoft.com/en-us/dotnet/api/system.int32.maxvalue).

## Usage Example:
```
using System;
using static Sisus.FlagsValues;

[Flags]
public enum MyEnum
{
  None	 = _0,
  First	 = _1,
  Second = _2,
  Third	 = _3,
  Fourth = _4,
  Fifth	 = _5
}
