
# WIX1002 Fundamentals of Programming

## Tutorial 4: Flow of Control (Repetition)

### Question 1: Write statements for each of the following.

#### (a) Find the largest integer n so that n³ is less than 2000.

```java
int n = 1;

while ((n + 1) * (n + 1) * (n + 1) < 2000) {
    n++;
}

System.out.println(n);
```

#### (b) Display the square number of the first twelve integers starting from 1.

```java
for (int i = 1; i <= 12; i++) {
    System.out.println(i * i);
}
```

#### (c) Display a 4-by-5 matrix using random numbers within 0 to 100.

```java
import java.util.Random;

Random generator = new Random();

for (int row = 1; row <= 4; row++) {
    for (int column = 1; column <= 5; column++) {
        System.out.printf("%4d", generator.nextInt(101));
    }
    System.out.println();
}
```

#### (d) Compute the sum of numbers from 1 to a given number.

```java
int sum = 0;

for (int i = 1; i <= number; i++) {
    sum += i;
}

System.out.println(sum);
```

#### (e) Compute the sum of the series: 1/25 + 2/24 + 3/23 + ... + 25/1 in two decimal places.

```java
double sum = 0.0;

for (int i = 1; i <= 25; i++) {
    sum += (double) i / (26 - i);
}

System.out.printf("%.2f%n", sum);
```


### Question 2: Correct the error for the following statements.

#### (a)

**Corrected statements:**

```java
for (x = 10; x > 0; x--)
    sum += x;
```

#### (b)

**Corrected statements:**

```java
do {
    x += 2;
    y += x;
    System.out.println(x + " and " + y);
} while (x < 100);
```

#### (c)

**Corrected statements:**

```java
for (x = 1, y = 20; x < y; x++, y -= 2)
    System.out.println(x + " " + y);
```

#### (d)

**Corrected statements:**

```java
i = 1;

while (i < 10) {
    if (i == 9)
        System.out.println("Program End");
    i++;
}
```


### Question 3: Write the statements that display the first ten values of the Fibonacci sequence. Given the formula f₁ = 1, f₂ = 1, fₙ = fₙ₋₁ + fₙ₋₂.

**Java statements:**

```java
int first = 1;
int second = 1;

System.out.print(first + " " + second + " ");

for (int i = 3; i <= 10; i++) {
    int next = first + second;
    System.out.print(next + " ");

    first = second;
    second = next;
}
```


### Question 4: Write the statements that display the string in reverse order. (Use `String.length()` to get the length of the string.)

**Java statements:**

```java
for (int i = str.length() - 1; i >= 0; i--) {
    System.out.print(str.charAt(i));
}
```
