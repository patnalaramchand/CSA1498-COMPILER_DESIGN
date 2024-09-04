# CSA1498-COMPILER_DESIGN

# Keyword or Identifiers
AIM-- Write a LEX program to check whether the given input is digit or not.

PROGRAM:: 
   
    %{
    %}

    %%

    main|if|else|return|while|dowhile|for|switch|break|call {printf("\nIt is Keyword\n");}

    [A-Za-z]|[a-zA-Z0-9]* {printf("\nIt is an Identifier\n");}

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

