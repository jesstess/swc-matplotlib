1. basic_plot.py
================

a) Examine and then run basic_plot.py. When pyplot.plot is given only
one list of values, it assumes they are y-values.

b) Change the plot to display lines between the data points:

    pyplot.plot([0, 2, 4, 8, 16, 32], "o")

becomes

    pyplot.plot([0, 2, 4, 8, 16, 32], "o-")

Change the labels, re-run the script, and note the changes in the
figure.

c) Add x-values to the data:

    pyplot.plot([0, 2, 4, 8, 16, 32], "o-")

becomes

    x_values = [3, 4, 7, 20, 22, 25]
    y_values = [0, 2, 4, 8, 16, 32]
    pyplot.plot(x_values, y_values, "o-")

Note how matplotlib resizes the graph to fit all the points on the
figure for you.

d) Instead of hard-coding values, use the random module to generate
random x and y values for basic_plot.py:
http://docs.python.org/library/random.html


2. world_population.py
======================

a) Examine and then run world_population.py. Look at the format of
world_population.txt.

b) Get a gist from this example about how reading from a file
works in Python, including:

- permissions (read, write, append)
- what the readlines function does
- what the split function does

Note that we are using the same pyplot functions from basic_plot.py.

c) Read about customizing plot lines at
http://matplotlib.sourceforge.net/api/pyplot_api.html#matplotlib.pyplot.plot

d) Change the arguments to pyplot.plot to make the world population
plot use a magenta, tri_down marker and a linewidth of 2.


3. Life expectancies
====================

a) In a new file, write code to plot the data in
life_expectancies_usa.txt. The format in this file is <year>,<male
life expectancy>,<female life expectancy>.

You can call pyplot.plot multiple times to draw multiple lines on the
same figure. For example:

  pyplot.plot(my_data_1, "mo-", label="my data 1")
  pyplot.plot(my_data_2, "bo-", "label="my data 2")

will plot my_data_1 in magenta and my_data_2 in blue on the same figure.

If you supply labels for your plots, like above, pyplot.legend will
display a legend for you graph.


4. constitution.py
==================

a) consitution.py plots the letter frequencies for the
Constitution. Run constitution.py. Note that the frequencies match our
intuition (or at least what Wheel of Fortune tells us) about the most
common letters in English.

b) Walk through constitution.py. Note how we are reading data from a
file this time, using read instead of readlines like in
world_population.py. Why?

c) The bar chart generation code is a substantial leap in complexity
from our previous plot. Focus on a broad-strokes understanding of what
the code is doing.

d) Use the same letter frequency plotting from constitution.py to
analyse the contents of mystery.txt. What is unusual about this
excerpt?
