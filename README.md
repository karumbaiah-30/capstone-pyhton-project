# capstone pyhton project
Data Preparation and Integration
The project began with understanding three core datasets: employee details (including personal and job information), project assignments (with cost and status), and seniority levels. Each dataframe contained unique and interconnected attributes such as employee ID, project costs, cities, ages, designation levels, and project statuses. The first major task was to join all three dataframes into a unified "Final" dataframe by merging on common keys, ensuring seamless analysis across different dimensions.

Analytical Transformations
Following the integration, a new bonus column was created in the final dataframe. This column allocated a 5% bonus based on project costs, but only for employees who had finished their respective projects, which required conditional logic and filtering entries where the project status was "Finished".

One of the advanced manipulations involved adjusting the designation levels. For employees whose projects were marked as "Fail," their designation level was demoted by 1. The dataset was further filtered by removing any employee records with a designation level above 4, aligning with business rules that restrict eligibility for heading projects.

Data Cleaning and Enrichment
To enhance presentation, titles ("Mr." or "Mrs.") were prefixed to first names, and the redundant gender column was dropped for conciseness and clarity. Designation levels were also promoted by 1 for employees older than 29, using an IF condition, thus demonstrating proficiency in additional pandas transformations.

Cost Aggregation and Specialized Views
Another significant achievement was aggregating project costs for each employee across all assignments. This was stored in a new dataframe titled "TotalProjCost," with employee ID, name, and their total project expenditure. Such aggregation required grouping and sum operations, providing an executive-level overview of financial contributions by staff members.

The project also featured advanced querying capabilities. As a final step, the solution printed all employee records where the city name contained the letter "o," utilizing string operations and logical filtering in pandas.

Skills Demonstrated
This capstone demonstrates proficiency in data merging, conditional logic, aggregation, string processing, and dataframe management—key skills for Python-based data analysis. It highlights expertise in cleaning, joining, filtering, and transforming tabular data to extract actionable business insights, making this project a valuable addition to any analytics portfolio.
