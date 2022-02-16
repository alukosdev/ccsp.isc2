# Investigation Process

## 1. Identify

Identify and preserve evidence and begin chain of custody documentation.

## 2. Collect

Label, record, acquire evidence, and ensure that modification does not occur.

1. Develop a plan to acquire the data; important factors for prioritization include:
   1. Likely value
   2. Volatility
   3. Amount of effort required
2. Acquire the data
3. Verify the integrity of the data

Network forensics has various use cases for data acquisition and collection:

* Uncovering proof of an attack
* Troubleshooting performance issues
* Monitoring activity for compliance with policies
* Sourcing data leaks
* Creating audit trails for business transactions

#### Prioritization of Volatile Data

1. Network connections
2. Login sessions
3. Contents of memory
4. Running processes
5. Open files
6. Network configuration
7. Operating system time

#### Alternative Prioritization

1. CPU cache, registers, RAM
2. Virtual memory
3. Disk drives
4. Backups and printouts

## 3. Examine

After data has been collected, the next phase is to examine the data, which involves assessing and extracting the relevant pieces of information from the collected data.

Yields data. Just the facts. For example:

- File opened at 10:23 AM
- DNS stopped at 7:02 AM
- etc.

## 4. Analyze

The analysis should include identifying people, places, items, and events and determining how these elements are related so that a conclusion can be reached.

Often, this effort includes correlating data among multiple sources. For instance, a NIDS log may link an event to a host, the host audit logs may link the event to a specific user account, and the host IDS log may indicate what actions that user performed.

How to identify who completed an event:

- Source address
- User identity \(if authenticated or otherwise known\)
- Geolocation
- Service name and protocol
- Window, form, or page \(such as URL address\)
- Application address
- Application identifier

Information. Taking data and putting it into context. For example:

- DNS stopped at 7:02 AM *but* nobody should have had access to DNS at 7:02 AM...

## 5. Report

The final phase is reporting, which is the process of preparing and presenting the information resulting from the analysis phase. Many factors affect reporting, including the following:

- Alternative explanations
- Audience consideration
- Actionable information

:::info
The ultimate recipient of all forensic evidentiary collection and analysis-the entity getting the reports-will be **the court**, in order to make a final determination of its merits and insights.
:::

## 6. Lessons Learned

Document what was learned. Something is always learned.