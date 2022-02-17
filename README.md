# GravityCalculator

**DESCRIPTION** 

In this assignment, you will create a program that computes the distance an object will fall in Earth's gravity. 

Modify the example program to compute the position of an object after falling for 10 seconds, outputting the position in meters

The formula in Math notation is: x(t) = 0.5 × at 2 + vit + xi Variable Meaning Value a Acceleration (m/s 2 ) -9.81 t Time (s) 10 vi Initial velocity (m/s) 0 xi Initial position 0

**Original Code**

```
class GravityCalculator {
    public static void main(String[] arguments) {
        double gravity = -9.81; // Earth's gravity in m/s^2
        double initialVelocity = 0.0;
        double fallingTime = 10.0;
        double initialPosition = 0.0;
        double finalPosition = 0.0;
        System.out.println("The object's position after " + fallingTime + " seconds is " + finalPosition + " m.");
    }
}

```

*Output of this code* 

![image](https://github.com/takara1215/GravityCalculator/blob/492dbd7dcf8acd7d356dc6d34f6b300292619412/Screenshot%202022-02-17%20140106.png)


**Modified Code**

```
public class GravityCalculator {

    public static void main(String[] arguments) {
        double gravity = -9.81; // Earth's gravity in m/s^2
        double initialVelocity = 0.0;
        double fallingTime = 10.0;
        double initialPosition = 0.0;
        double x;

        x = (0.5 * gravity*(fallingTime*fallingTime)
                + (initialVelocity * fallingTime) + (initialPosition));

        System.out.println("The object's position after " + fallingTime + " seconds is " + x + " m.");
    }
}
```


*Output of this code*

![image](https://user-images.githubusercontent.com/85555680/154259684-2b623a18-09bb-41fa-a812-cec27dd7e8b6.png)

