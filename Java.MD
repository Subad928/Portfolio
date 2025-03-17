# Java If and Boolean Logic

## Introduction
This document explains Java if-statements and boolean expressions with example code and exercises. It also references CodingBat live boolean logic practice problems for additional hands-on learning.

## If Statement
An if-statement controls which parts of the code execute based on boolean conditions.
```java
if (temperature > 100) {
  System.out.println("Dang, it's hot!");
}
```

## If-Else Statement
Used for either-or logic, where one of two possible actions is executed.
```java
if (temperature > 100) {
  System.out.println("Too darn hot");
} else {
  System.out.println("At least it's not more than 100");
}
```

## Java Comparison Operators
Comparison expressions evaluate to boolean values:
- `<` less-than
- `>` greater-than
- `<=` less-or-equal
- `>=` greater-or-equal
- `==` equality
- `!=` not equal

Example:
```java
if (score < 100) {
  System.out.println("Keep going!");
}
```

## Boolean Operators
Boolean expressions use logical operators:
- `&&` (AND) evaluates to true if both expressions are true.
- `||` (OR) evaluates to true if at least one expression is true.
- `!` (NOT) inverts a boolean value.

Example:
```java
if ((score >= 10) && (temperature >= 100)) {
  System.out.println("It's hot out, and so am I!");
}
```

## Boolean Type
Booleans store true or false values.
```java
boolean isHot = true;
boolean isCold = false;
```

## Boolean Short-Circuiting
Expressions stop evaluating as soon as the result is known.
```java
if (i != 0 && (100.0 / i < 10.0)) {
  System.out.println("Valid division");
}
```

## Boolean Methods
Methods that return boolean values:
```java
public boolean isLowFuel() {
  return ((myGasoline + myBattery) < 10);
}
```

## Nested If-Statements
An if-statement inside another if-statement:
```java
if (day <= 5) {
  System.out.println("Weekday");
  if (day == 1) {
    System.out.println("It's Monday!");
  }
} else {
  System.out.println("Weekend");
}
```

## If-Else Chains
Handles multiple conditions:
```java
if (score >= 300) {
  System.out.println("Perfect!");
} else if (score >= 200) {
  System.out.println("Very good");
} else if (score >= 50) {
  System.out.println("Good job");
} else {
  System.out.println("Keep practicing!");
}
```

## Boolean Puzzles
Example boolean logic exercises:
```java
public void test(int num, boolean bool) {
  if (num >= 90 || !bool) {
    System.out.println("A");
  } else {
    System.out.println("B");
  }
}
```

## Floating Point Comparisons
Avoid using `==` for doubles due to precision errors:
```java
if (Math.abs(d1 - d2) <= 1e-6) {
  System.out.println("Values are nearly equal");
}
```

## Conclusion
Boolean logic and if-statements form the foundation of decision-making in Java programs. Understanding boolean expressions, logical operators, and best practices for writing clean code enhances programming efficiency.

_Copyright 2012 Nick Parlante_