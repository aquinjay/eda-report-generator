# EDA Report Generator
This script helps users automaticaly generate exploratory data analysis reports to get to know their data.

This code base relies on 3 modules to generate reports:
- [Ydata](https://ydata-profiling.ydata.ai/docs/master/index.html)
- [Dataprep](https://dataprep.ai)
- [Sweetviz](https://github.com/fbdesignpro/sweetviz)

There is reduendancy between reports but they all have their own flavors that make it nice to use all three.

### Requirements
After making your virtual environment, you will need to install the following modules:
- click
- os
- pandas
- dataprep
- ydata-profiling
- sweetviz

Be sure to use a python version equal to or before 3.10.6 but after 3.7. 3.10.6 worked for me.

### How to use

Open the command line (not tested on windows machines yet) and run:
`python report-generator.py file_name`

You can also generate individual reports using the report flag:
`python report-generator.py file_name --report ydata`

You can also pass dataprep or sweetviz instead. By default all reports are generated.

So far csv, xlsx, json, and pkl files are supported. Will consider and test for more as needed.
