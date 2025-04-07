# Midterm Exam for Econ 138: Data Science for Economists
April 2025

## General Instructions
- This is an open-book, open-notes, and open-internet exam.
- You may consult any resource, but **all code and analysis must be your own**.
- Collaboration with others is **strictly not allowed**.
- Copy-pasting code or using generative AI tools without understanding is a violation of academic integrity.
- Violations will result in a failing grade and further disciplinary action.
- **Deadline:** April 11, 2025 at 8:00 PM Philippine Standard Time (no extensions unless granted in advance).

## Submission Instructions
- Submit your exam as a **Jupyter notebook** named `midterm_exam.ipynb`.
- Place your notebook in the root directory of this repo (same folder as this README).
- Your pull request must include:
  - A working `midterm_exam.ipynb`
  - A short note in the pull request message linking to your GitHub profile (e.g., `https://github.com/yourusername`)
- Make sure to **push your changes** before the deadline.
  
## Exam Instructions
1. Set a global file path
- define a global file path variable `file_path` that points to the directory where you will save your files.
- also define a global variable `data_path` that points to the directory where you will save your data files.
- the file path should be a string that points to the directory where you will save your files.

2. Load the data
- load the data from the `data_path` variable.
- The FIES data are too large for GitHub. You may download them instead [here](https://drive.google.com/drive/u/3/folders/17DSHWyN-3D-RRbbCWTwBbjVCgV8t1SPn).
- load all the FIES files into separate dataframes.
- for the geodata files, use the shape files from `https://data.humdata.org` on your local machine, given that the files are too large.

3. Inspect the data
- inspect the data to see what columns are available.
- inspect the data to see what the data types are.
- Use the relevant functions to understand the formats, missing values, and the categories of the data.

4. Exploratory Data Analysis
- for each FIES year, illustrate the distribution of the 'total income', 'total expenditure', 'family size', and 'per capita income'
- Create a table that shows the value counts for each region and province. (i.e. province should be nested under region)
- Create profiles for each region by showing the mean and median income and expenditure for each province nested under the region.

5. Merge the data
- merge the data into a single dataframe.
- based on the data inspection, decide which columns to keep and which columns to drop to merge the data.
- clean the data if necessary.
- make sure to create a new column that indicates the year of the data.

6. Additional Analysis of the Merged Data
- For each region, illustrate the composition of income and expenditure of each household, on average.
- Calculate the implied savings rate for each region and province, on average. Map where there are savings and where there are deficits using a choropleth map.
- Create a demographic profile of the regions and provinces by showing the mean and median family size, income, and expenditure for each region and province.
- Create a rank for the top and bottom 10 provinces based on the average income and expenditure.
- Compare the growth rates of income and expenditure for each region and province.

You are encouraged to go beyond the required tasks by exploring:
- What income sources drive the most inequality?
- Are regions becoming more or less reliant on remittances?
- Is there a link between family size and income dynamics?

Note that these are just the bare minimum requirements. You are free to add any additional analysis that you think would be relevant or interesting. You are also free to use any libraries or tools that you think would be useful. You are also free to use additional data sources if you think they would be useful. The goal of the exam is to demonstrate your ability to analyze and visualize data, so feel free to be creative and use your own judgment in how you approach the analysis.


## Additional Instructions
- Write a short explanation for each major block of code using **Markdown cells**.
- Comment your code clearly and use meaningful variable names.
- Structure your notebook cleanly (use headers and sections).
- Your goal is to **communicate insights**, not just execute code.
