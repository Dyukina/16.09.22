# 16.09.22
## Задание 1
---
You will be given an array a and a value x. All you need to do is check whether the provided array contains the value.

Array can contain numbers or strings. X can be either.

Return true if the array contains the value, false if not.

### Решение 
```java
public class Solution {
    public static boolean check(Object[] a, Object x) {
        for (int i = 0; i < a.length; i++) {
    if (a[i].equals(x))
return true;
}
return false;
}
}
```
### Любимое решение
```java
import java.util.Arrays;

public class Solution {

    public static boolean check(Object[] a, Object x) {
        return Arrays.asList(a).contains(x);
    }

}
```


## Задание 2
---
You've just moved into a perfectly straight street with exactly n identical houses on either side of the road. 
 Naturally, you would like to find out the house number of the people on the other side of the street.

### Решение
```java
class CodeWars {
        public static long overTheRoad(long address, long n) {
        long inv = 1 + n * 2;
        return inv - address;
    }
}
```
### Любимое решение
```java
class CodeWars {
public static long overTheRoad(long address, long n) {

return (n * 2) - (address - 1);

  }
}
```

