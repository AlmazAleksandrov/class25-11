### Task 8kyu:

Now you have to write a function that takes an argument and returns the square of it.

[Task link](https://www.codewars.com/kata/523b623152af8a30c6000027/train/java)

#### Solution:
```
public class Kata
{
    public static int square(int n){
        return n*n;

    }
}
```

#### Fav solution:
```
public class Kata
{
    public static int square(int n){
        return (int) Math.pow(n, 2);
    }
}
```

#### Comment:
It is difficult to come up with some original solution. Too simple a task.

### Task 7kyu:

Find the total sum of internal angles (in degrees) in an n-sided simple polygon. N will be greater than 2.

[Task link](https://www.codewars.com/kata/5a03b3f6a1c9040084001765/train/java)

#### Solution:
```
public class AngleSum {
    public static int sumOfAngles(int n) {
        return 180*(n-2);
    }
}
```

#### Fav solution:
```
public class AngleSum {
    public static int sumOfAngles(int n) {
        if(n == 3)
            return 180;
        if(n == 4)
            return 360;
        return 180 + sumOfAngles(n-1);
    }
}
```

#### Comment:
Added two conditions, complicated the code. My solution is definitely better.
