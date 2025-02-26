# Convert the test cases into Markdown format

markdown_content = """# TEST CASES - Apache Iceberg and Trino Containers using Podman

## Submitted By
Manish Kumar Chaudhary

## Submitted To
<Reviewer Name>

## Test Case Version
1.0

## Reviewer Name
<Reviewer Name>

---

## Goal
The objective of this project is to set up Apache Iceberg and Trino containers using Podman on Ubuntu. The setup includes inserting 100,000 records into Iceberg, connecting Trino with Iceberg, and performing SQL queries to demonstrate efficient data management and querying capabilities.

---

## Table of Contents
- [Test Environment](#test-environment)
- [TC1: Iceberg-Spark Container Startup](#tc1-iceberg-spark-container-startup)
- [TC2: Trino Container Startup](#tc2-trino-container-startup)
- [TC3: Data Insertion in Iceberg](#tc3-data-insertion-in-iceberg)
- [TC4: Data Retrieval using Iceberg](#tc4-data-retrieval-using-iceberg)
- [TC5: Data Retrieval using Trino](#tc5-data-retrieval-using-trino)
- [TC6: Data Consistency Check](#tc6-data-consistency-check)
- [TC7: Complex Query Execution](#tc7-complex-query-execution)
- [TC8: Negative Test Cases](#tc8-negative-test-cases)
- [NFR Test Cases](#nfr-test-cases)

---

## Test Environment
The testing environment includes Apache Iceberg and Trino containers running on Podman in Ubuntu. 
The Iceberg container uses Spark for data operations, while Trino is used for querying and data integration.

---

## TC1: Iceberg-Spark Container Startup
### Scenario
Verify that the Apache Iceberg-Spark container starts successfully.

### Remarks: 
N/A

### Given
- The Iceberg-Spark image is pulled using Podman.

### When
- The container is started with required ports and configurations.

### Then
- The container should be running and accessible.

### Test Run
- **Date:** 
- **Result:** Pending/Pass/Fail

### Testing outputs  
*(Paste your output/snapshots here)*

---

## TC2: Trino Container Startup
### Scenario
Verify that the Trino container starts and connects to Iceberg.

### Remarks: 
N/A

### Given
- The Trino image is pulled and configured with Iceberg catalog.

### When
- The container is started with the configuration mounted.

### Then
- The container should be running, and Trino should connect to Iceberg.

### Test Run
- **Date:** 
- **Result:** Pending/Pass/Fail

### Testing outputs  
*(Paste your output/snapshots here)*

---

## TC3: Data Insertion in Iceberg
### Scenario
Verify data insertion of 100,000 records in Iceberg.

### Remarks: 
N/A

### Given
- The Iceberg table is created using Spark.

### When
- 100,000 records are inserted using a loop in Spark Shell.

### Then
- All records should be inserted successfully.

### Test Run
- **Date:** 
- **Result:** Pending/Pass/Fail

### Testing outputs  
*(Paste your output/snapshots here)*

---

## TC4: Data Retrieval using Iceberg
### Scenario
Verify data retrieval using Spark Shell.

### Remarks: 
N/A

### Given
- Data is inserted into the Iceberg table.

### When
- A SELECT query is executed to retrieve data.

### Then
- Data should be retrieved without errors.

### Test Run
- **Date:** 
- **Result:** Pending/Pass/Fail

### Testing outputs  
*(Paste your output/snapshots here)*

---

## TC5: Data Retrieval using Trino
### Scenario
Verify data retrieval using Trino CLI.

### Remarks: 
N/A

### Given
- Trino is configured to use Iceberg as a catalog.

### When
- A SELECT query is executed in Trino CLI.

### Then
- Data should be retrieved consistently with Iceberg.

### Test Run
- **Date:** 
- **Result:** Pending/Pass/Fail

### Testing outputs  
*(Paste your output/snapshots here)*

---

## TC6: Data Consistency Check
### Scenario
Check data consistency between Spark and Trino queries.

### Remarks: 
N/A

### Given
- Data is inserted using Spark.

### When
- Data is queried using both Spark and Trino.

### Then
- Data count and values should be consistent.

### Test Run
- **Date:** 
- **Result:** Pending/Pass/Fail

### Testing outputs  
*(Paste your output/snapshots here)*

---

## TC7: Complex Query Execution
### Scenario
Test the performance of complex queries.

### Remarks: 
N/A

### Given
- Data is available in Iceberg.

### When
- Complex queries with filters, joins, and aggregations are executed.

### Then
- Queries should execute efficiently without errors.

### Test Run
- **Date:** 
- **Result:** Pending/Pass/Fail

### Testing outputs  
*(Paste your output/snapshots here)*

---

## TC8: Negative Test Cases
### Scenario
Verify system behavior with invalid inputs.

### Remarks: 
N/A

### Given
- Invalid data types and non-existent tables are queried.

### When
- Queries are executed using Spark and Trino.

### Then
- Appropriate error messages should be displayed.

### Test Run
- **Date:** 
- **Result:** Pending/Pass/Fail

### Testing outputs  
*(Paste your output/snapshots here)*

---

## NFR Test Cases
Test performance, scalability, and security of the Apache Iceberg and Trino setup. 
Includes stress testing for large datasets and security testing for access controls.
"""

# Save the Markdown content to a file
output_md_file = '/mnt/data/Apache_Iceberg_Trino_Test_Cases.md'
with open(output_md_file, 'w') as file:
    file.write(markdown_content)

output_md_file
