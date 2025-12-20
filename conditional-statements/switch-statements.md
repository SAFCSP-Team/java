# Switch Statement 

The `switch` statement is a conditional control structure that allows you to select and execute one of several code blocks based on the value of a single expression. It makes your code clearer and easier to read than using multiple `if-else if` statements.


## Syntax

```java
switch (expression) {
    case value1:
        // Code to run if expression == value1
        break;
    case value2:
        // Code to run if expression == value2
        break;
    // ... more cases ...
    default:
        // Code to run if no case matches
}
```

### How a `switch` Statement Works

- You provide the `switch` statement with an **expression** (usually a variable).
- The program compares the value of this expression to each `case` value.
- If a case matches, its code block executes.
- The `break` statement ends the current case and exits the `switch`.
- Optionally, you can add a `default` block, which runs if none of the cases match.


## Example

```java
int day = 3;
String dayName;

switch (day) {
    case 1:
        dayName = "Sunday";
        break;
    case 2:
        dayName = "Monday";
        break;
    case 3:
        dayName = "Tuesday";
        break;
    case 4:
        dayName = "Wednesday";
        break;
    case 5:
        dayName = "Thursday";
        break;
    case 6:
        dayName = "Friday";
        break;
    case 7:
        dayName = "Saturday";
        break;
    default:
        dayName = "Invalid day";
}
System.out.println(dayName);
```

**Output**
```
Wednesday
```

## The `break` Statement

- The `break` statement ends the execution of the current case and exits the `switch`.
- If you delete the `break` statement, **the program will continue executing the code for subsequent cases** (known as "fall-through").
- In the last case or the `default` case, a `break` statement is not required.

### Example of Fall-Through:

```java
int number = 2;

switch (number) {
    case 1:
        System.out.println("One");
    case 2:
        System.out.println("Two");
    case 3:
        System.out.println("Three");
        break;
    case 4:
        System.out.println("Four");
}
```
**Output**
```
Two
Three
```


## The `default` Case

The `default` case is **optional** but recommended. It executes if none of the cases match the expression, similar to the `else` block in an `if-else` statement.

### Example

```java
int month = 13;

switch (month) {
    case 1:
        System.out.println("January");
        break;
    case 2:
        System.out.println("February");
        break;
    // ... other months ...
    default:
        System.out.println("Not a valid month!");
}
```

**Output:**
```
Not a valid month!
```











