# Coding Journal - Adrian R

I'm Adrian and this is my journal, where I write by sessions following the blockchain developer roadmap.
## Ambitions and goals
I'm studying to become a blockchain developer within the next....


<!--- This is a new entry -->
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


<!--- This is a new entry -->
## nov 10, 2022
> "Excellence withers without an adversary." — Seneca

### Day intro
Today I worked on the final project for CoderHouse - Web Development, I have to clean up the SASS code and ensure style is done for desktop / media queries and what ever is remaining.

### Problems encountered
The first problem was that the mixin and include broke, so I had to check why it wasn't working.

The second problem section html tag was being used incorrectly.

The third the mixin/include breaks the npm run watch-css script

### Solutions explored
For the SASS issue, I searched first why it could have broken, but it appeared that the code was correct.

For the usage of the section tag, searched on the correct usage and how to style semantic tags.

For the third, I have not check what the issue was.
### Successful solutions
For the SASS issue, I just re-typed the code and the issue was resolved, I'm not sure why it broke.

For the section, I left the semantic tags unstyled and applied style only to the divs.
### Revisit
I revisited SASS mixin and include tags and usage of semantic tag.

### Lessons learned
For the SASS issue, sometimes staff breaks, does not mean I'm wrong, trying again is a viable solution.

For the semantic tags, I learned that those are left unstyled, and I only focused on the divs for that purpose.


<!--- This is a new entry -->
## nov 12, 2022
> "First say to yourself what you would be; and then do what you have to do." — Epictetus

### Day intro
Today I worked again on the final project for CoderHouse - Web Development, I was able to wrap it up, finish the SASS and upload it.

### Problems encountered
I was not happy with the layout and how Bootstrap was deployed so I decided to review it.

### Solutions explored
I basically review the Bootstrap framework  and how container, container-fluid, row and column are handled and assigned.
### Successful solutions
After re-arranging the grid, I fixed all the other pages and was easy after that.
### Revisit
I revisited the Bootstrap framework and SASS variables to finish cleaning up the code.

### Lessons learned
How to apply Bootstrap tags for main grid and practice setting variables, using mixins and includes.

Markdown Guide
https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

https://yushi95.medium.com/how-to-create-a-beautiful-readme-for-your-github-profile-36957caa711c

<!--- This is a new entry -->
## nov 29, 2022
> "I will keep constant watch over myself and‚ most usefully‚ will put each day up for review." — Seneca

### Day intro
Today I worked on the Credit exercise for CS50.

### Problems encountered
I left the code mid-way, and uncommented, I had to re-read and re-write. Also, I had to learn how to use get_long and actually get it to print for testing. I also had issued using and printing modulo and I have an issue about the code asking twice for entry.

### Solutions explored
I looked at the possible uses for get_long and found the CS50 Manual less-comfortable version, which provide more detailed information.
### Successful solutions
After properly implementing get_long, I was able to print to test the function. I'm still trying to figure out the double input request, I believe if has to do with the void parameter.
### Revisit
I found the CS50 Manual, and along google searches I got it to work, I'm avoiding postings specific to CS50 exercise.

### Lessons learned
Testing helps to avoid problems further down, also writing pseudocode or instructions prior to solution helps to outline the action plan.