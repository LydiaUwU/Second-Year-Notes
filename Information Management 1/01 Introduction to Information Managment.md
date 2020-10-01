# Introduction to Information Management

## Some Core Concepts
**Organisation:** How data is represented/associated.
**Metadata:** Data about what the data is.
**Access:** How to interact with the data efficiently.

## What is the Difference Between Data, Information and Knowledge
**Data:**
- Raw; Building blocks of information.
- Unprocessed information.

**Information:**
- Data associated together to convey some meaning.
- Basic unit of communication.

**Knowledge:**
- Interrelating and "understanding" information.

## Maintaining Structure in Your Own Data File
Files just represent data as a series of bytes and will *lose the structure* that you might have imposed either logically or physically unless you do something about it.

There are many ways of adding structure to files, for example:
- **Delimited-text Field:** Choose a special character/delimiter that will not appears as a legitimate character within the information field and then insert that character into the file after writing each field.
- **Fixed-length Field:** Use a fixed length for each information field and pad out when the length of the actual data value is less than the fixed length.
- **Length-based Field:** Write the length of the value of the information field followed by the value in exactly that number of bytes.
- **Identified Field:** Write the name of the information field and then value both represented as delimited-text fields.

## Turning Data into information
There are two distinct approaches:
- **Structured Approach:** Deliberately associate data together to turn it into information. *E.g. excel, databases, etc.*
- **Unstructured Approach:** Bring loosely managed data together to serve specific information needs using information retrieval techniques. *E.g. search engines.*

## Nature of Querying
**Structured:** Uses artificial language with known data types and exact criteria.
**Unstructured:** Keyword and phrase based.

## Nature of Results
**Structured:**
- Returns definitive results.
- Returns the complete set of data that meets search criteria.
- No estimation of relevancy

## Structured Approach Specialist Software
### Databases (DBs)
- A combination of software and hardware.
- Optimised to reduce data to storage transfer.
- Optimised to provide Transactional/ACID (Atomic, Consistent, Isolated, Durable).
- Designed to be administered and secure.
- Different Models:
  - Relational.
  - Networked.
  - Hierarchical.
  - Object-oriented

### DataWarehouses (DWs)
DataWarehouse is a subject oriented, integrated, nonvolatile, time-variant collection of data in support of management's decisions.

DataWarehouse is a repository of data which is:
- Separate from operational systems and populated by data from these systems.
- Provides a trend view of data.
- Available entirely for the task of making data available to be interrogated by business users.
- **Timestamped** and associated with defined periods of time.
- Accessible to users who have a limited knowledge of computer systems or data structures.

Used for:
- Data mining.
- Decision Support.
- OLAP.

## Unstructured Approach Specialist Software
### Information Retrieval
Fundamental concerns:
- Efficient Access.
- "Relevant" results through matching

## Common Challenges managing data for Enterprises and Individuals
**Variety:** Data extends beyond structured data, including semi-structured and unstructured data of all varieties.
**Volume:** There is an insane amount of data in the world.
**Velocity:** Often time-sensitive, data must be processed as it is streaming in order to maximise its value.
**Validity:**
- **Data Protection:** Consent and compliance.
- **Data Privacy:** What data an individual is willing to share.
- **Data Ethics:** Consideration of ethical issues when processing data.

## Solution Trend for Velocity: "Big Data"
**Realtime** analytic techniques and technologies are becoming increasingly important, *requires rapid data access*.

## Solution Trend for Volume: "The Cloud"
Desire to "out source" information management and technologies to massively distributed computing resources.

## Solution Trend for Validity
### Protection
In Europe GDPR challenges explicit gathering and lifecycle management.

### Privacy
Raising awareness and providing tools for users to understand the "convenience vs privacy" tradeoff.

### Ethics
Conversation just beginning on the ethics of processing data.
Being taken seriously at a corporate level (*E.g. IDM*) **THIS IS FUCKING TERRIFYING**
Efforts ongoing to provide stakeholders to address ethics early in development cycle.
