---
title: Notes for Flex and Bison
date: 2019-09-19
categories:
- book-reading
tags:
- compiler design
---

## Notes for Flex and Bison

needed for course: practice of compiler design

a simple word count ==> done!
- gcc lex.yy.c -lfl
- actually has a default rule of .  ECHO
    - turn off by %option nodefault

```c
%{
int chars = 0;
int words = 0;
int lines = 0;
%}
%%
[a-zA-Z]+ { words++; chars += strlen(yytext); }
\n { chars++; lines++; }
. { chars++; }
%%
main(int argc, char **argv)
{
yylex();
printf("%8d%8d%8d\n", lines, words, chars);
}
```

BNF grammars
- no need to reduce left resursion?
- bison reports conflict when ambiguity detected
- bison only handle LL(1) or LR(1) grammar?

include bison generated .h file in .l file

well i found this
- http://westes.github.io/flex/manual/
- for reference when implmenting compiler for mini-c
- start states
    - kind of like that in automata
    - diff. state defines diff. scanners

yyterminate: return immediately

only with % yylineno will flex maintain yylineno
- still need to initialize to 1 manually

important(?) regex from pp.38/58

Bison
- for most of the cases, only LALR(1) supported
- no ambiguity, no more than one look ahead char.
- create a union for AST
    - declare which token holds which value
    - and need to assign corresponding value in .l file
- define precedence in bison
    - %left, %right

define user function
- user function also parsed to a AST

left recursive better in bison
- right recursive cause large stack

skip Chap. 4 for SQL parsing
