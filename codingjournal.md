# Coding Journal - Adrian R

I'm Adrian and this is my journal, where I write by sessions following the blockchain developer roadmap.
## Ambitions and goals
I'm studying to become a blockchain developer within the next....



## nov 7, 2022
> "Dwell on the beauty of life. Watch the stars, and see yourself running with them." —Marcus Aurelius

### Day intro
Currently I'm working on the PSET 1 for CS50, I started by doing the mario-less version.

### Problems encountered
For the mario-less version I found that I could print the dots and hashes but the number was off by one.

### Solutions explored
For mario-less version I tried to manipulate the variable setting in each for loop but it would either blank out or duplicate the number.

### Successful solutions
For mario-less the solution was to apply arithmetic operations in both the variable setting and the condition evaluation.

### Revisit
I had to revisit the for-loop in C to be further understand and attempt next pset.

### Lessons learned
For mario-less I did not know one could have nested for-loops at the same level within the function. I also did not know that one could have arithmetic operations within the variable, evaluation and execution statements (the three parts within the parenthesis). I learned this by reading another solution, but then while reviewing the solution I learned that for-loops will run at least once (one iteration) if the evaluation is true and that if parent's loop variable is used in the next for-loop, its value is set to the starting value.

```
// This is my version of the Mario game

#include <cs50.h>
#include <stdio.h>

int main(void)
{
    // Initializes the variable for height
    int height;
    // Aks for user input in a specific range
    do
    {
        height = get_int("Pick a number from 1 to 8: ");
    } while (height < 1 || height > 8);

    // Loops over the height variable (pyramid size) and prints a new line (these are the rows)
    for (int i = 0; i < height; i++)
    {
        // Loops over each pyramid row's size and prints a period in each space for all lines
        // starting from 7 which is height - (i = 0) - 1 = 7 because 8 - 0 - 1 = 7 then reduces
        for (int j = height - i - 1; j > 0; j--)
        {
            printf(" ");
        }
        // Loops over each piyramids row's size and print a hash starting from 1
        // since (i = 0) + 1 = 1 then increases
        for (int k = 0; k < i + 1; k++)
        {
            printf("#");
        }

        printf("\n");
    }
}
```


Markdown Guide
https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

https://yushi95.medium.com/how-to-create-a-beautiful-readme-for-your-github-profile-36957caa711c