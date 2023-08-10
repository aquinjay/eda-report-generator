# EDA Report Generator
This script helps users automaticaly generate exploratory data analysis reports to get to know their data.

If you find this project helpful, consider staring this repo or making a donation to support this and future projects here via GitHub Sponsers: https://github.com/sponsors/aquinjay. 

This code base relies on 3 modules to generate reports:
- [Ydata](https://ydata-profiling.ydata.ai/docs/master/index.html)
- [Dataprep](https://dataprep.ai)
- [Sweetviz](https://github.com/fbdesignpro/sweetviz)

Check them out if you want to tinker, clean, and explore beyond the scope of this script.
Note, there is reduendancy between reports but they all have their own flavors that make it nice to view all three.

### Requirements
After making your virtual environment, you will need to install the following modules:
- click
- dataprep
- ydata-profiling
- sweetviz

Be sure to use python version 3.10.

### How to use

Clone the repo and copy the `report_generator.py` file or copy and paste the `report_generator.py` file into the directory your data is located in.
Open the command line and cd into your working directory (not tested on windows machines yet) and run:
```cmd
python report-generator.py file_name
```

You can also generate individual reports using the report flag:
```cmd
python report-generator.py file_name --report ydata
```

You can also pass `dataprep` or `sweetviz` instead. By default all reports are generated.

So far csv, xlsx, json, and pkl files are supported. Will consider and test for more as needed.
