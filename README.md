This project demonstrates how to create the Koch Snowflake fractal using recursion in Java. 

## What happens at each recursive step?

1. Each line segment is divided into three equal parts.
2. A new equilateral triangle is created using the middle third as the base, pointing outward.
3. The original segment is replaced by four smaller segments: 
   - The left third of the original segment.
   - The left side of the new triangle.
   - The right side of the new triangle.
   - The right third of the original segment.
4. This process repeats for every segment until the recursion depth is reached.

## Base Case

The recursion stops when the recursion depth equals the maximum level (`maxLevel`). At this point, the program simply draws a straight line segment.

## Using `translate()` and `rotate()`

- **`translate()`**: To center the Koch Snowflake within the canvas, the program translates the origin to the center of the window before drawing.
- **`rotate()`**: While rotation isn't strictly necessary for this implementation, it can be used to manipulate triangle orientation dynamically for variations of the snowflake.


