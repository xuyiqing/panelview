# panelView 1.1.18

1. Fix bugs with `collapse.history`.

2. Set `shade.post = FALSE` by default.

# panelView 1.1.17

Add links to the [JSS paper](https://doi.org/10.18637/jss.v107.i07).

# panelView 1.1.16

1. Add `collapse.history` to allow users to collapse unit by treatment history in a `treat` plot.

2. Add `show.missing` to output missing data summary statistics for the key variables. 

3. Add `axis.lab.angle` to allow users to change the angle of the axis labels on the x-axis.

3. Allow `pre.post` to be applied to an `outcome` plot.

4. Change the color scheme in the `outcome` plot.

5. Fix bugs.

# panelView 1.1.11

1. Add `by.cohort` to allow users to plot the average outcome trajectories of units with the same treatment history (if the number of unique treatment history is less than 20).

2. The old version (v.1.1.6) can be found [here](https://yiqingxu.org/packages/panelview/panelView_1.1.6.tar.gz); its user's guide [here](https://yiqingxu.org/packages/panelview/panelView_1.1.6.html). 

# panelView 1.1.10

1. Add `by.group.side` to arrange subfigures of `by.group = TRUE` in a row rather than in a column.

2. Add `display.all` to show all units if the number of units is more than 500, otherwise we randomly select 500 units to present.

# panelView 1.1.8

1. Add a new option `leave.gap` to keep gaps in time using white bars when the time variable is not evenly distributed (possibly due to missing data).

2. Add `type(missing)` to plot the missingness in data. 

# panelView 1.1.7

1. We replace the function name *panelView* with *panelview* to be consistent with the Stata version. 

2. In the outcome plot, we use a dot to represent the last-period observation of a unit that gets treated in the last period.

# panelView 1.1.6

Plot time series of outcome and treatment in one graph (`type = "bivar"`). The default is to plot mean D and Y against time in the same graph. To plot by each specified unit, add option  `by.unit = TRUE`. Use  `style = c("","")` to set line/connected line/bar styles for the outcome and treatment variables and  `ylim = list(c( , ), c( , ))` to zoom in or out the figure. `lwd` is for line width adjustment. 

# panelView 1.1.4

Add a new option `treat.type` to control whether the treatment variable should be seen as a continuous (`treat.type = "continuous"`) or discrete (`treat.type = "discrete"`) variable. 

# panelView 1.1.2

1. Change the plot `type`: we now use `"treat"` (`"missing"` in earlier versions) to plot treatment status and `"outcome"` (`"raw"` in earlier versions) to plot raw outcomes. 
2. Allow >2 treatment levels.
3. Add a new option `pre.post` to distinguish pre- and post-treatment observations for treated units in a DID setting.
4. Replace options `by.treatment` with `by.timing` and `treatment` with `ignore.treat` for easier interpretations.
5. Add fontsize options.

# panelView 1.0.5

Fix typos. CRAN release.

# panelView 1.0.4

1. Allow users to plot treated units on top of control units in the "missing" plot.
2. Streamline the `color` option for both the "missing" and "raw" plots. 

# panelView 1.0.3

1. Allow users to change the color of bricks in the "missing" plot.
2. Allow users to leave the treatment blank in both the "missing" and "raw" plots. 
