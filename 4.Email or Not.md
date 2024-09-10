# CSA1498-COMPILER_DESIGN

# Valid Email or Not
AIM-- Write a LEX program to check whether the given input is Email or not.

PROGRAM:: 

    %{
    %}

    %%

    [a-z.A-Z0-9_]+"@"[a-z]+".com"|".in" {printf("\nIts a Valid Email_id: \n");}
    .+ {printf("\nNot a Valid Email\n");}

    %%
    int yywrap(void) {}

    int main()
    {
    printf("\nEnter string : ");
    yylex();
    printf("\n");
    return 0;
    }
OUTPUT::

![Exp 5](https://github.com/user-attachments/assets/28d7b223-199e-469c-881b-2228f6aa4d50)
