# CSA1498-COMPILER_DESIGN

# No.of Vowels and Consonents
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
![Exp 4](https://github.com/user-attachments/assets/66ef88b3-882c-443f-ae2d-59e1a49f6049)

