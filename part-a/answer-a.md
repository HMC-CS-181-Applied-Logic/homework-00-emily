## Part a

### Describe what the code in `z3-test.py` is doing in a paragraph or two.

`z3-test.py` first intializes two boolean variables (`a` and `b`) and two integer variables (`x` and `y`). The first part of the program determines if the logical expression `And(Not(a), b, x > 0, x < 100, x < y)` is satisfiable. As it is satisfiable, it prints `sat` as well as a solution (`x = 99, y = 100, b = True, a = False`) for the variables that satisfy the expression. This, however, is not the only solution, but it does use the largest values that the integer variables `x` and `y` can be. The program then adds a constraint, `y < 1`, making the set of expressions unsatisfiable (`unsat`).
