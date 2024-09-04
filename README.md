# CSA1498-COMPILER_DESIGN

[EXPERIMENT-1]
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

![exp 1](https://github.com/user-attachments/assets/b94e58f7-1477-44d1-9b42-d61959325905)
