# ADD LINE
PROGRAM:

    %{
    int ln=0;
    %}

    %%

    .* {ln++;fprintf(yyout,"\n%d:%s",ln,yytext);}

    %%
    int yywrap(void) {}

    int main()
    {
    yyin=fopen("mul.txt","r");
    yyout=fopen("outnew.txt","w");
    yylex();
    }

OUTPUT:
