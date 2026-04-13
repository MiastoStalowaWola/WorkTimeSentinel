## Working Time Sentinel

## Project Overview

**Working Time Sentinel** is an automated access control system based on data retrieved from a Time and Attendance (RCP) system.

The application integrates with **Active Directory** and **Microsoft 365** to enforce access policies derived from approved working time records, absences, and overtime authorizations. Its primary goal is to ensure that user access to IT resources is available **only when formally authorized**, in accordance with organizational security policies.

The system significantly reduces security risks, eliminates manual account handling, and supports compliance with information security regulations.

---

## Key Features

### RCP Integration
- Retrieval of **approved absences** (leave, sick leave, and other authorized absences).
- Retrieval of **approved overtime**.
- Processing only finalized and approved records (no draft or pending requests).

### Access Control (Active Directory / Microsoft 365)
- **Automatic blocking of user accounts** during approved absences.
- **Automatic blocking of access outside working hours**, unless approved overtime exists.
- **Automatic unblocking of accounts**:
  - before the start of the working day,
  - after the end of an absence period.

### Administrative Overrides and Exceptions
- Manual definition of **exceptions to blocking rules**, including:
  - selected user accounts,
  - defined time periods,
  - special organizational circumstances.
- Manual **forced blocking of selected accounts**, independent of RCP data (e.g. security incidents, administrative decisions).

### Automation and Security
- Scheduled and automated synchronization processes.
- Enforcement of the principle of least privilege in time-based access.
- Reduction of risks related to:
  - compromised accounts,
  - unauthorized after-hours access,
  - human error in manual account administration.

---

## Example Use Cases

- An employee has approved leave → their AD and Microsoft 365 accounts are automatically blocked for the duration of the leave.
- An employee attempts access outside working hours without approved overtime → access is denied.
- An employee has approved overtime → after-hours access is permitted.
- An administrator adds a temporary exception → automatic enforcement rules are bypassed for the defined scope.
- Beginning of a workday → access is automatically restored.

---

## Intended Audience

- public administration bodies,
- local government entities,
- organizations requiring strict access control,
- environments subject to NIS2, KSC, or internal information security policies.

---

## Licensing

The project is distributed as open-source software.  
Modified versions redistributed further must be published along with their source code, in accordance with the terms of the license.

See the `LICENSE` file for details.

---

## Project Status

Under active development.  
Integration interfaces and business logic may evolve over time.



## Authors
Marek Brzuchnalski
Administrative Assistant for IT / Software Developer
Stalowa Wola, Poland


Marcin Uszyński  
City Secretary / Head of Department  
Stalowa Wola, Poland

