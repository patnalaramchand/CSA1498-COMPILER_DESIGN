# CSA1498-COMPILER_DESIGN

# Mobile No. or Not
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
