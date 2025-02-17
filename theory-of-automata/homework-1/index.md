# Homework One

**Question 1**: Proving by contradiction.
$$(1 + 10)^∗\ and\ 1^∗ (101^∗)^{∗}$$
Assume $$L_1 = Language (1 + 10)^*$$ and $$L_2 = 1^∗ (101^∗)^{∗}$$
To prove by contradiction that the two regular expressions $$ \( (1 + 10)^{*} \) and \( 1^{*}(101^{*})^{*} \) $$ do not represent the same language, we assume they are equal and derive a contradiction.

$$ L_1 $$
   - $$ L_1 $$ $$ \( 1 + 10 \)^{*} $$ has for example these strings in  language: $$ \( \epsilon, 1, 10, 11, 1010, 1110, 101010, \) $$ etc.

- Consider the string **1001**:
    - 10 is a valid unit, and another 01 is not permitted in the construction from $$ \( (1+10)^{*} \) $$.
    - So 1001 is **not** in $$ \( (1 + 10)^{*} \) $$.
  
    - $$ \( 1^{*} \) $$ can generate a leading 1.  
    - $$ \( (101^{*})^{*} \) $$ can generate 101, forming 1001.
    - Hence, 1001 is in $$ \( 1^{*}(101^{*})^{*} \) $$ but **not** in $$ \( (1 + 10)^{*} \) $$.

We assumed that the two languages were equal, but we found a string 1001 that belongs to one but not the other. This contradicts our assumption.

**Question 2**: Showing that languages are star-free.
- (a). $$ (01)^{*}, { \epsilon, 01, 0101, 010101 ... } $$
- (b). $$ (01, 10)^{*} $$ cannot create strings that start with or end with 00, 11.

**Question 3**: $$ L_1 = {\ w\ :\ w begins\ with\ 1\ and\ ends\ with\ 0\ and\ has\ odd\ length\ } $$
