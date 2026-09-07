# C-Day-41-Count-Even-Odd-Digits
# C Day 41 - Count Even and Odd Digits

This program counts the total number of even and odd digits in a given number.

## Example

Input:

```text
58321
```

Output:

```text
Even digits = 2
Odd digits = 3
```

## Concepts Used

* while loop
* if-else
* Modulus operator (%)
* Division operator (/)
* Digit extraction
* Counter variables

## How It Works

1. Extract the last digit using `% 10`.
2. Check whether the digit is even or odd.
3. Increase the appropriate counter.
4. Remove the last digit using `/ 10`.
5. Repeat until all digits are checked.

## C Code

```c
#include <stdio.h>

int main()
{
    int num, digit;
    int even = 0, odd = 0;

    printf("Enter a number: ");
    scanf("%d", &num);

    while (num != 0)
    {
        digit = num % 10;

        if (digit % 2 == 0)
        {
            even++;
        }
        else
        {
            odd++;
        }

        num = num / 10;
    }

    printf("Even digits = %d\n", even);
    printf("Odd digits = %d", odd);

    return 0;
}
```

## Output

```text
Enter a number: 58321
Even digits = 2
Odd digits = 3
```
