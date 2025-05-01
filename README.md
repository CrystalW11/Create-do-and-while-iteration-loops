# Create-do-and-while-iteration-loops

### Use the continue statement to step directly to the Boolean expression

1. In certain cases, we want to short-circuit the remainder of the code in the code block and continue to the next iteration. We can do that using the `continue` statement.

```
Random random = new Random();
int current = random.Next(1, 11);

do
{
    current = random.Next(1, 11);

    if (current >= 8) continue;

    Console.WriteLine(current);
} while (current != 7);

/*
while (current >= 3)
{
    Console.WriteLine(current);
    current = random.Next(1, 11);
}
Console.WriteLine($"Last number: {current}");
*/
```

#### output

5
1
6
7