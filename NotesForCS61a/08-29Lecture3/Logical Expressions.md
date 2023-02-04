Logical expressions have corresponding evaluation procedures. These procedures exploit the fact that the truth value of a logical expression can sometimes be determined without evaluating all of its subexpressions, a feature called _short-circuiting_.

To evaluate the expression <left> and <right>:

1.  Evaluate the subexpression <left>.
2.  If the result is a false value v, then the expression evaluates to v.
3.  Otherwise, the expression evaluates to the value of the subexpression <right>.

To evaluate the expression <left> or <right>:

1.  Evaluate the subexpression <left>.
2.  If the result is a true value v, then the expression evaluates to v.
3.  Otherwise, the expression evaluates to the value of the subexpression <right>.

To evaluate the expression not <exp>:

1.  Evaluate <exp>; The value is True if the result is a false value, and False otherwise.

These values, rules, and operators provide us with a way to combine the results of comparisons. Functions that perform comparisons and return boolean values typically begin with is, not followed by an underscore (e.g., isfinite, isdigit, isinstance, etc.).