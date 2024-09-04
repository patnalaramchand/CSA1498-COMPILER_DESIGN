# CSA1498-COMPILER_DESIGN

[EXPERIMENT-1]
AIM-- Write a LEX program to check whether the given input is Identifier or not.

PROGRAM:: 


    %{
    %}

    %%

    [a-zA-Z][a-zA-Z0-9]+ {printf("\nIdentifier is  Valid\n");}
    .+ {printf("\nIdentifier is Invalid\n");}
    %%
    int yywrap(void) {}

    int main()
    {
    printf("\nEnter Identifier : ");
    yylex();
    printf("\n");
    return 0;
    }

OUTPUT::
