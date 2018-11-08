# CS50-Mario-Less-Comfortable

build a half pyramid in the mario world


#include <stdio.h>
#include <cs50.h>


int main(void)
{
    int height;
    
    //Prompt user to enter Postitive number no greater than 23
    do
    {
        height = get_int("Positive Number: ");
    }
    while (height <= 0 || height > 23);

    for (int line = 0; line < height; line++)
    {
        for (int space = height - line; space > 1; space--)
        {
            printf(" ");
        }
        
        for (int block = 0; block < line + 2; block++)
        {
            printf("#");
        }
        
        printf("\n");
    }

    
}
