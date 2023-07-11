# improvado-analyse

This project aims to analyze activity data and identify the most vulnerable process based on event timestamps. The analysis is performed using Python and various data analysis libraries.

## Dataset

The dataset used for this analysis consists of event data captured during various processes. The structure of the dataset is as follows:

- `case_id`: Identifier for each case or process.
- `timestamp`: Timestamp of the event.
- `event`: Type of event that occurred.
- `duration`: Duration of the event in days.
- `metadata`: Additional metadata associated with the event.

## Process Descriptions

The dataset contains events from different processes. Here are brief descriptions of each process:

- **Process Start**: The initial event that marks the start of a process.
- **Contact Created**: Creation of a contact, typically with information about the contact's job title or role.
- **User Session**: A user session on the website, including details about the traffic source and medium.
- **Lead Created**: Creation of a lead or potential customer.
- **Disco Call Book**: Recording an appointment for a discovery call.
- **End Process**: The final event that marks the end of a process.

## Project Steps

1. **Data Preparation**: The dataset is loaded into a suitable data structure for analysis, such as a Pandas DataFrame.

2. **Activity Visualization**: An activity schema is created based on the data using a visualization tool like Celonis. The activity schema provides a visual representation of the flow of activities and their relationships.

3. **Timestamp Analysis**: The timestamps of events are analyzed to calculate the time differences between consecutive events in each process. This analysis helps identify the duration of each process.

4. **Identifying the Most Vulnerable Process**: The process with the highest duration or other vulnerability indicators is identified as the most vulnerable process.

5. **Report and Insights**: A comprehensive report is generated summarizing the project work, including dataset description, activity schema, timestamp analysis results, and the identification of the most vulnerable process. The report concludes with insights and recommendations based on the analysis.

## SQL Query

To further analyze the dataset, a SQL query can be executed to extract additional information from the data. Here is an example SQL query that retrieves the total count of events for each process:

```sql
SELECT event, COUNT(*) AS event_count
FROM your_table_name
GROUP BY event;

## Getting Started

To run the project and reproduce the analysis, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/activity-analysis-project.git
