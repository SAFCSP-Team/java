
# Conditional Statements (if, else if, else, switch)

## `if` Statement

Executes a block of code if a specified condition is true.

```java
if (condition) {
    // code to be executed if condition is true
}
```

**Example**

```java
int score = 75;
if (score >= 60) {
    System.out.println("You passed the exam.");
}
```
**Output**
```
You passed the exam.
```

## `if-else` Statements

Executes one block of code if the condition is true, and another block if the condition is false.

```java
if (condition) {
    // code to be executed if condition is true
} else {
    // code to be executed if condition is false
}
```

**Example**
```java
int age = 17;
if (age >= 18) {
    System.out.println("You are an adult.");
} else {
    System.out.println("You are a minor.");
}
```
**Output**
```
You are a minor.
```

### Ternary Operator
The ternary operator is a shorthand for the if-else statement. It uses the `?` and `:` symbols.

```java
variable = (condition) ? valueIfTrue : valueIfFalse;
```
**Example**
```java
int age = 17;
String result = (age >= 18) ? "You are an adult." : "You are a minor.";
System.out.println(result);
```
**Output**
```
You are a minor.
```
The ternary operator is a concise way to perform conditional assignments or evaluations.

## `else if` Statement

Used to test multiple conditions.

```java
if (condition1) {
    // code to be executed if condition1 is true
} else if (condition2) {
    // code to be executed if condition2 is true
} else {
    // code to be executed if none of the conditions are true
}
```

**Example**

```java
int time = 20;
if (time < 12) {
    System.out.println("Good morning.");
} else if (time < 18) {
    System.out.println("Good afternoon.");
} else {
    System.out.println("Good evening.");
}
```
**Output**
```
Good evening.
```

## `switch` Statement

Selects one of many code blocks to be executed. It is often a more efficient alternative to long `if-else if` chains when you are testing a single variable against multiple possible values.

```java
switch (expression) {
    case value1:
        // code block
        break;
    case value2:
        // code block
        break;
    default:
        // code block
}
```

*   The `expression` is evaluated once.
*   The value of the `expression` is compared with the values of each `case`.
*   If there is a match, the associated block of code is executed.
*   The `break` keyword is used to exit the `switch` block. If `break` is omitted, execution will continue to the next `case`.
*   The `default` keyword is optional and specifies the code to run if there is no case match.

**Example**

```java
int day = 4;
String dayName;

switch (day) {
    case 1:
        dayName = "Monday";
        break;
    case 2:
        dayName = "Tuesday";
        break;
    case 3:
        dayName = "Wednesday";
        break;
    case 4:
        dayName = "Thursday";
        break;
    case 5:
        dayName = "Friday";
        break;
    case 6:
        dayName = "Saturday";
        break;
    case 7:
        dayName = "Sunday";
        break;
    default:
        dayName = "Invalid day";
}
System.out.println(dayName);
```
**Output**
```
Thursday
```


