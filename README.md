###  [Task 8kyu](https://www.codewars.com/kata/5748838ce2fab90b86001b1a/train/java)

Complete the function that calculates the area of the red square, when the length of the circular arc A is given as the input. Return the result rounded to two decimals.
### My solution
```Java
public class Geometry{
    public static double squareArea(double A){
        double B = 2* A / Math.PI;
        B *= B;
        String formattDouble = String.format("%.2f", B);
        B = Double.parseDouble(formattDouble);
        return B;
    }
}
```

### Fav solution

```Java
public class Geometry{
    public static double squareArea(double A){
        double l = (2*A)/Math.PI;
        double x = l*l;
        double y = Math.round(x * 100) * 0.01d;
        return y;
    }
}

```
I like this solution because I like it
