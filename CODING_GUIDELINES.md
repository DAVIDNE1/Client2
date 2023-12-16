
# Coding Rules

## 1. Code Formatting

### 1.1 Indentation

Use 4 spaces for indentation. Do not use tabs.

```java
// Good
public class MyClass {
    public static void main(String[] args) {
        // code here
    }
}

// Bad - Using tabs
public class MyClass {
    public static void main(String[] args) {
		// code here
    }
}
```

### 1.2 Braces

Place opening braces `{` on the same line as the declaration and closing braces `}` on a new line.

```java
// Good
public class MyClass {
    public static void main(String[] args) {
        if (condition) {
            // code here
        } else {
            // code here
        }
    }
}

// Bad - Opening brace on a new line
public class MyClass 
{
    public static void main(String[] args) 
    {
        if (condition) 
        {
            // code here
        } 
        else 
        {
            // code here
        }
    }
}
```

## 2. Naming Conventions

### 2.1 Classes and Interfaces

Use CamelCase for class and interface names.

```java
// Good
public class CalculatorService {
    // code here
}

// Bad - Not using CamelCase
public class calculator_service {
    // code here
}
```

### 2.2 Variables and Methods

Use camelCase for variable and method names.

```java
// Good
int calculateSum(int a, int b) {
    // code here
}

// Bad - Not using camelCase
int calculate_sum(int a, int b) {
    // code here
}
```

## 3. Comments

### 3.1 Inline Comments

Use inline comments sparingly and ensure they add value to the code. Keep them concise.

```java
// Good
int result = a + b; // Calculate the sum

// Bad - Redundant comment
int result = a + b; // Add a and b to get the result
```

### 3.2 Block Comments

Use block comments to explain complex code sections or provide context.

```java
/*
 * This method performs a complex calculation to determine the final result.
 * It takes into account various factors and conditions.
 */
int calculateResult() {
    // code here
}
```

## 4. Exception Handling

Handle exceptions appropriately and avoid using broad exception catch clauses.

```java
// Good
try {
    // code that may throw an exception
} catch (SpecificException e) {
    // handle SpecificException
} catch (AnotherException e) {
    // handle AnotherException
}

// Bad - Catching a broad exception
try {
    // code that may throw an exception
} catch (Exception e) {
    // handle any exception
}
```

## 5. Miscellaneous

### 5.1 Constants

Use `static final` for constants, and use uppercase letters with underscores.

```java
// Good
public static final int MAX_VALUE = 100;

// Bad - Not using uppercase letters or underscores
public static final int maxvalue = 100;
```

### 5.2 Code Organization

Organize your code logically into packages and classes. Avoid putting too much functionality into a single class.

```java
// Good
package com.example.calculator;

public class Calculator {
    // code here
}

// Bad - Overly complex class
public class MyApplication {
    // code here
}
```
