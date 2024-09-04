# CSA1498-COMPILER_DESIGN

# [EXPERIMENT-1]
AIM-- Write a LEX program to check whether the given input has no.of vowls and consonents.

PROGRAM:: 
  
    %{
    int vow_count=0;
    int con_count=0;
    %}

    %%

    [AEIOUaeiou] {vow_count++;}

    [a-zA-Z] {con_count++;}

    %%
    int yywrap(void) {}
 
    int main()
    {
    printf("\nEnter input : ");
    yylex();
    printf("\nNo. of vowels: %d\n",vow_count);
    printf("\nNo. of consonents: %d\n",con_count);
    return 0;
    }

OUTPUT::

