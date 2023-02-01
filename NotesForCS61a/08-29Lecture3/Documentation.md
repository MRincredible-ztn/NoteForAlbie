A function definition will often include documentation describing the function, called a _docstring_, which must be indented along with the function body. Docstrings are conventionally triple quoted. The first line describes the job of the function in one line. The following lines can describe arguments and clarify the behavior of the function:

>>> def pressure(v, t, n):
        """Compute the pressure in pascals of an ideal gas.

        Applies the ideal gas law: http://en.wikipedia.org/wiki/Ideal_gas_law

        v -- volume of gas, in cubic meters
        t -- absolute temperature in degrees kelvin
        n -- particles of gas
        """
        k = 1.38e-23  # Boltzmann's constant
        return n * k * t / v

When you call help with the name of a function as an argument, you see its docstring (type q to quit Python help).

>>> help(pressure)

When writing Python programs, include docstrings for all but the simplest functions. Remember, code is written only once, but often read many times. The Python docs include [docstring guidelines](http://www.python.org/dev/peps/pep-0257/)that maintain consistency across different Python projects.

**Comments**. Comments in Python can be attached to the end of a line following the # symbol. For example, the comment Boltzmann's constant above describes k. These comments don't ever appear in Python's help, and they are ignored by the interpreter. They exist for humans alone.