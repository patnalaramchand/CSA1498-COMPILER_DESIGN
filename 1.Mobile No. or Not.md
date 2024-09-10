# CSA1498-COMPILER_DESIGN

# Valid Mobile No. or Not
AIM-- Write a LEX program to check whether the given input is VALID Mobile number or not.

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
![exp 1](https://github.com/user-attachments/assets/0ce823cb-983b-4f42-b6f9-05ae50dbec5d)
