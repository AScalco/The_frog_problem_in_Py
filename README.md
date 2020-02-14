# The frog problem in Py
A solution to the frog problem made in Python along with some basic analyses

### Credits

The following description of the frog problem was originally proposed by Dr. Christie Lee from the Robert Gordon University during the Aberdeen Python User Group MeetUp of February 2020. The Jupyter Notebook contains my solution to the problem. An analysis of the average number of hops depending on the maximum number of lily pads is also reported using Panda and Matplotlib packages.

## The Frog Problem
  
This problem requires you to write a simulation of a system involving randomness.

A frog wants to get from it's current lily pad (pad `0`) to another lily pad `n` pads are (pad `n`)

For example, if `n=4`, there are 5 total pads (0 to 4).

The frog can hop as far as it wants in a single bound! But it likes to randomly choose any of the lily pads in front of it (with equal probability) and hop to that one.

Once hopped, it again, randomly chooses any of the lily pads in front of it (with equal probability) and hops to that.

When it reaches lily pad `n` (in this case 4), the frog is home.

The frog can take in total anywhere between 1 and n hops to get home.

First, write a function which simulates the frog's journey once. The parameter `n` is the distance the frog has to travel (1 less than the number of pads).

**Since it is random, it will vary from run-to-run!!!**

Example usage:

    >>> simulate_frog(4):
    2

    >>> simulate_frog(4):
    2

    >>> simulate_frog(4):
    1

    >>> simulate_frog(4):
    3

Next, add a named parenter which allows your function to repeate the simulation many times and return the average (mean) number of hops the journey took.

    >>> simulate_frog(4, simulations=1000000):
    2.082791

The answer will vary, but you should get around `2.08` for `n=4`.

Fill in the table with the results from your simulation, and try to find a pattern.

| n         | Average Number of Hops |
| --------: | ---------------------: |
| 0         | 0 |
| 1         | 1 |
| 2         | ... |
| 3         | ... |
| 4         | ~ 2.08 |
| 5         | ... |
| ... | ... |

Work out how many hops it will take on average for `n = 1,000,000` (Hint: compare each entry in the table above to the previous row to work out a formula)

Use a plotting library to generate a plot with `n` on the x-axis and Average number of hops on the y-axis. Try plotting on the smae chart, both your simulation results, and prediction for an explicit formula and see how they match up!

</details>
