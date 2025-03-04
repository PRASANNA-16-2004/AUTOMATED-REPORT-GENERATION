# AUTOMATED-REPORT-GENERATION

 *COMPANY*: CODETECH IT SOLUTIONS PVT.LTD
 
 *NAME*: PERUMALLA LAKSHMI PRASANNA
 
 *INTERN ID*: CT08PRF
 
 *DOMAIN*: Python programming
 
 *DURATION*: 4 Weeks
 
 *MENTOR*: Neela Santosh Kumar


Overview of the Code
The script follows a systematic approach:

Loads student data from an Excel file
Creates bar graphs for subject scores
Generates a structured PDF report
These reports help visualize the student’s performance over time in different subjects.

Detailed Explanation of the Code
1. Importing Required Libraries
The script starts by importing the necessary libraries. Pandas is used for handling student data in a tabular format, while Matplotlib is responsible for generating bar graphs that compare subject scores over different months. ReportLab is used to create structured PDF reports. Additionally, the script includes the OS module to check for file existence and handle file paths.

2. Creating a Bar Graph from Student Data
The function responsible for creating the bar graph reads the student data file and extracts relevant information, such as months, Science scores, and Arts scores. If the file is empty or missing, the function prints a warning and exits to avoid errors in subsequent steps.

The extracted data is then used to generate a bar graph, where Science scores are represented by blue bars and Arts scores by red bars. Labels are added to the x-axis, y-axis, and title for clarity. The month labels are rotated for better readability. The generated graph is then saved as an image, which will be used later in the report.

The function includes error handling mechanisms for missing files, incorrect column names, or unexpected issues that may arise while processing the data.

3. Generating the PDF Report
The function responsible for generating the PDF report begins by defining the page size and inserting a title at the top of the document. It then formats the textual content to ensure clear and readable output.

After inserting the textual content, the function checks whether the bar graph image file exists. If the image is available, it is inserted into the PDF; otherwise, a warning is displayed, and the script proceeds without the image. Finally, the report is saved as a PDF file, and a success message is printed to confirm its creation.

To prevent errors during execution, the function includes an exception handling mechanism that catches unexpected issues that may arise while generating the report.

4. Processing Multiple Students in a Loop
The script processes four students in a loop, automating the creation of individual reports for each one.

It first verifies whether the Excel file containing student data exists. If the file is missing, an error message is displayed, and the script moves to the next student. The script then loads the specific sheet corresponding to the current student and converts the data into a CSV file for further processing.

Once the CSV file is created, the script calls the function responsible for generating a bar graph, passing the file as input. After the graph is successfully created, the function responsible for generating the PDF report is called, incorporating the generated graph into the final document.

If the script encounters a missing sheet within the Excel file, an error message is displayed, and the script continues processing the remaining students. Exception handling is also implemented to catch and report any unexpected errors that may occur during execution.

Key Features of the Script

✔ Automates Report Generation – Processes multiple students in a loop.

✔ Visualizes Student Performance – Generates bar graphs for clarity.

✔ Handles Missing Files Gracefully – Prevents crashes with error handling.

✔ Saves Reports in PDF Format – Provides a structured output for analysis.

Support & Learning: Throughout the project, I leveraged ChatGPT for assistance in debugging errors, and improving visualization techniques. It provided solutions to common issues and helped refine the workflow.

Conclusion:
This script automates student performance report generation using Python, pandas, matplotlib, and ReportLab. It loads data from an Excel file, creates bar graphs, and generates PDF reports with detailed insights. The error handling ensures smooth execution even when data is missing.

This approach can be extended to larger datasets, different subjects, and other types of analysis. It’s an efficient way to visualize and document performance trends over time.

*Output*

![Image](https://github.com/user-attachments/assets/71df0de6-d092-4df8-849a-27fcc9b6721b)

