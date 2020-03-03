#### Question
 * Try to find the flag

#### Hint
 * Nothing

#### Solution
- Encoded Text

 *KysrKysrKysrK1s+Kz4rKys+KysrKysrKz4rKysrKysrKysrPDw8PC1dPj4+LS0tLS0tLS0tLS0t
LS0tLisuCisrKysrKysrKytbPis+KysrPisrKysrKys+KysrKysrKysrKzw8PDwtXT4+KysrKysr
KysrKysrKysrKysrKy4uLgorKysrKysrKysrWz4rPisrKz4rKysrKysrPisrKysrKysrKys8PDw8
LV0+PisrKysrKysrKysrKysrKysrKysuLisrKysrKysuCisrKysrKysrKytbPis+KysrPisrKysr
Kys+KysrKysrKysrKzw8PDwtXT4+Pi0tLS0tLS0tLS0tLS0uLS0uCisrKysrKysrKytbPis+Kysr
PisrKysrKys+KysrKysrKysrKzw8PDwtXT4+KysrKysrKysrKysrKysrKysrKy4rLisuCisrKysr
KysrKytbPis+KysrPisrKysrKys+KysrKysrKysrKzw8PDwtXT4+Pi0tLS0tLS0tLS0tLS0tLS0u
LS4KKysrKysrKysrK1s+Kz4rKys+KysrKysrKz4rKysrKysrKysrPDw8PC1dPj4+LS0tLS0tLS0t
LS0tLS0tLS0tLS4rKysuCisrKysrKysrKytbPis+KysrPisrKysrKys+KysrKysrKysrKzw8PDwt
XT4+Pi0tLS0tLS0tLS0tLS0tLS0uKy4KKysrKysrKysrK1s+Kz4rKys+KysrKysrKz4rKysrKysr
KysrPDw8PC1dPj4+LS0tLS0tLS0tLS0tLS0tLi0tLS0uCisrKysrKysrKytbPis+KysrPisrKysr
Kys+KysrKysrKysrKzw8PDwtXT4+Pi0tLS0tLS0tLS0tLS0uLS0tLS4KKysrKysrKysrK1s+Kz4r
Kys+KysrKysrKz4rKysrKysrKysrPDw8PC1dPj4+LS0tLS0tLS0tLS0tLS4uCisrKysrKysrKytb
Pis+KysrPisrKysrKys+KysrKysrKysrKzw8PDwtXT4+Pi0tLS0tLS0tLS0tLS0tLS0tLS4rKysr
LgorKysrKysrKysrWz4rPisrKz4rKysrKysrPisrKysrKysrKys8PDw8LV0+PisrKysrKysrKysr
KysrKysrKysuLS4uCisrKysrKysrKytbPis+KysrPisrKysrKys+KysrKysrKysrKzw8PDwtXT4+
Pi0tLS0tLS0tLS0tLS0tLS0tLi0tLS0uCisrKysrKysrKytbPis+KysrPisrKysrKys+KysrKysr
KysrKzw8PDwtXT4+KysrKysrKysrKysrKysrKysrKy4rLisrKy4K*

```$ cat kysrk | base64 -d```

*++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>>---------------.+.
++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>+++++++++++++++++++...
++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>+++++++++++++++++++..+++++++.
++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>>-------------.--.
++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>+++++++++++++++++++.+.+.
++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>>----------------.-.
++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>>-------------------.+++.
++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>>----------------.+.
++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>>---------------.----.
++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>>-------------.----.
++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>>-------------..
++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>>------------------.++++.
++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>+++++++++++++++++++.-..
++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>>-----------------.----.
++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>+++++++++++++++++++.+.+++.*

- We got 16 lines of brainfuck code and the decoded numbers are

*Output = 78, 111, 118, 97, 123, 65, 36, 67, 73, 73, 95, 99, 48, 100, 51, 125]*

```
numbers = [78, 111, 118, 97, 123, 65, 36, 67, 73, 73, 95, 99, 48, 100, 51, 125]
flag = []
for i in numbers:
  flag.append(chr(i))
print(''.join(flag))
```
