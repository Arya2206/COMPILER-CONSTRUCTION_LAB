# exp10_1219 — For Loop Syntax Validator (Lex & Yacc)

Validates the syntax of a C-style `for` loop using Lex and Yacc.

## Files
- `exp10_1219.l` — Lex file (tokenizer)
- `exp10_1219.y` — Yacc file (grammar rules)


## Build & Run

```bash
yacc -d exp10_1219.y
lex exp10_1219.l
gcc y.tab.c lex.yy.c -o exp10_1219 -ll
./exp10_1219
```

## Sample Output

```
Enter a for loop:
for(i=0; i<10; i++)
Valid for loop
```

```
Enter a for loop:
for(i=0 i<10; i++)
Invalid for loop
```
