# CSA1498-COMPILER_DESIGN

# Digit or Not
AIM-- Write a LEX program to check whether the given input is digit or not.

PROGRAM:: 

    %{
    %}
    %%
    [6-9][0-9]{9} {printf("\nMobile Number  Valid\n");}
    .+ {printf("\nMobile Number Invalid\n");}
    %%
    int yywrap(void) {}
    int main()
    {
    printf("\nEnter Mobile Number : ");
    yylex();
    printf("\n");
    return 0;
    }
OUTPUT::
![exp 2](https://github.com/user-attachments/assets/33d24b03-2671-4525-bd4f-16ffed5ed898)

