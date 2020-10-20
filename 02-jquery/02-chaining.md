# Method Chaining
jQuery makes extensive use of a pattern called **method chaining**.

## The Problem
Imagine a `Car` object in JavaScript.  This `Car` object has the following methods:
| Method         | Signature             |
|----------------|-----------------------|
| startEngine()  | () -> undefined       |
| turnLeft()     | () -> undefined       |
| turnRight()    | () -> undefined       |
| moveForward(n) | (Number) -> undefined |
| stopEngine()   | () -> undefined       |

If we wanted to use the `Car` we might write code that looks similar to this.

```js
var volkswagen = new Car(); // NOTE: We haven't learned about this type of object creation -- yet.
volkswagen.startEngine();
volkswagen.moveForward(-1);
volkswagen.turnRight();
volkswagen.moveForward(2);
volkswagen.turnLeft();
volkswagen.moveForward(1);
volkswagen.turnLeft();
volkswagen.moveForward(8);
volkswagen.stopEngine();
```

## A Solution
Method chaining would require each of these methods return the car object itself back to the caller.

These signatures would now look like this:
| Method         | Signature       |
|----------------|-----------------|
| startEngine()  | () -> Car       |
| turnLeft()     | () -> Car       |
| turnRight()    | () -> Car       |
| moveForward(n) | (Number) -> Car |
| stopEngine()   | () -> Car       |

What this allows the caller to do is chain the function calls one after the other.

```js
var volkswagen = new Car()
  .startEngine()
  .moveForward(-1)
  .turnRight()
  .moveForward(2)
  .turnLeft()
  .moveForward(1)
  .turnLeft()
  .moveForward(8)
  .stopEngine();
```
