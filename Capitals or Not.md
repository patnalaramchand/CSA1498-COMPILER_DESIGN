# CSA1498-COMPILER_DESIGN

# Capitals or Not
AIM-- Write a LEX program to check whether the given input is Capitals or not.

PROGRAM:: 

    %{ 
    %}

    %%

    [A-Z]+ {printf("\nIt is a Capital word\n");}

    .+ {printf("\nnot a Capital word\n");}
 
    %%
    int yywrap(void) {}

    int main()
    {
    printf("\nEnter String : ");
    yylex();
    printf("\n");
    return 0;
    }
OUTPUT:
