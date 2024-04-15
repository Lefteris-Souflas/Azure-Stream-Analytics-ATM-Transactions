# Modern Data Management & Business Intelligence

Assignment 3 for the Data Management and Business Intelligence Course of AUEB's MSc in Business Analytics

## Description

In this assignment, you will utilize Azure Stream Analytics to process a data stream of ATM transactions and answer stream queries. Follow the steps below to complete the assignment:

### Steps:

1. **Create a Student Account:**
    - Register for a student account at [Azure for Students](https://azure.microsoft.com/en-us/free/students/).

2. **Setup Event Hub:**
    - Configure an Event Hub in Azure.

3. **Generate Security Access Signature:**
    - Generate a Security Access Signature using [RedDog](https://github.com/sandrinodimattia/RedDog/releases) in a terminal (Windows OS).

4. **Edit Generator.html:**
    - Update the `CONFIG` variables in Generator.html using a text editor (e.g., Sublime or Notepad++).

5. **Feed Event Hub:**
    - Utilize Generator.html to feed data into the Event Hub.

6. **Setup Storage Account:**
    - Configure a Storage account in Azure.

7. **Upload Reference Data Files:**
    - Upload the reference data files (e.g., AREA.json, ATM.json, Customer.json) to your Azure Storage account.

8. **Setup Stream Analytics Job:**
    - Create a Stream Analytics Job in Azure.

9. **Define Inputs:**
    - Use the Event Hub and reference data files as input for the Stream Analytics Job.

10. **Create Output:**
    - Configure Blob Storage as the output for the Stream Analytics Job.

### Scenario:

You have access to a data stream generated from ATMs, containing transaction-related data. Your task is to create an Azure Analytics solution to handle the following queries:

### Queries:

1. Show the total amount of Type=0 transactions at ATM Code=21 of the last 10 minutes (using a sliding window).
2. Show the total amount of Type=1 transactions at ATM Code=21 of the last hour (using a tumbling window).
3. Show the total amount of Type=1 transactions at ATM Code=21 of the last hour, repeating once every 30 minutes (using a hopping window).
4. Show the total amount of Type=1 transactions per ATM Code of the last hour (using a sliding window).
5. Show the total amount of Type=1 transactions per Area Code of the last hour, repeating once every hour (using a tumbling window).
6. Show the total amount per ATM's City and Customer's Gender of the last hour, repeating once every hour (using a tumbling window).
7. Alert (SELECT "1") if a Customer has performed two Type=1 transactions in an hour window (using a sliding window).
8. Alert (SELECT "1") if the ATM's Area Code doesn't match the Customer's Area Code (using a sliding window).

### Deliverable:

A .pdf document detailing the process of setting up your account and executing the queries, including screenshots of each step and output files. Ensure to start each job and include screenshots of the output files.
