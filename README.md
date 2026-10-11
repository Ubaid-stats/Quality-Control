# X-bar and R Charts for a Manufacturing Process

This project builds X-bar and R control charts for a hard-bake process
in semiconductor manufacturing. It is written in R Markdown.

## About the project
In semiconductor manufacturing, the flow width of the resist (in microns)
is an important quality measure. This project checks whether the process
is in statistical control.

- Number of samples: 25
- Wafers in each sample: 5 (125 measurements in total)
- Samples were taken every one hour

## What the project does
1. Finds the mean and range of each sample.
2. Finds the grand mean and the average range.
3. Calculates the control limits (UCL, CL, LCL) for both charts.
4. Draws the X-bar chart and the R chart.
5. Checks for points outside the control limits.

## Result
Both charts show no out-of-control points and no unusual pattern.
So the process is in statistical control, and the trial control limits
can be used to monitor future production.

## Files
- `file.Rmd`: R Markdown file with the code and the full analysis
- `file.pdf`: The final report (output of the Rmd file)

## How to run
1. Install R and RStudio.
2. Open `file.Rmd` in RStudio.
3. Click the **Knit** button to make the report.

Note: the PDF output needs a LaTeX setup (for example, the `tinytex`
package). To install it, run:
install.packages("tinytex")
tinytex::install_tinytex()

## Author
Ubaid
