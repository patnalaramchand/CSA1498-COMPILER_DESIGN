%{
float op1=6,op2=7;
%}
%%
"+" {printf("sum=%lf",op1+op2);}
"-" {printf("difference=%lf",op1-op2);}
"*" {printf("multiplication=%lf",op1*op2);}
"/" {printf("division=%lf",op1/op2);}
. {printf("enter proper operator.");}
%%
int yywrap() {}
int main() 
{
  printf("enter operator:");
  yylex();
}
