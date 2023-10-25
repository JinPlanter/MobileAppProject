Table of Contents:
* [Architectural Decision Record (ADR) - Database Storage](#architectural-decision-record-adr-database-storage)
    * [Context](#context)
    * [Decision](#decision)
    * [Rationale](#rationale)
    * [Consequences](#consequences)

<br/>

# Architectural Decision Record (ADR) - Database Storage

## Context

Tasked with the goal of creating a <font color=#61dafb>React Native</font> <font color=#9063CD>daily expenses tracker</font> for <font color=#3ddc84>Android</font> devices, our group must choose whether to go database-less or use a database storage that is {local/remote} and {encrypted/unencrypted}.

[comment]: # "const [isSelected, setIsSelected] = useState(false);"
[comment]: # (const databaseLocation = local || remote;)
[comment]: # (const encryptionState = encrypted || unencrypted;)

<br/>

## Decision

We have decided to use MariaDB as locally hosted encrypted backend.

<br/>

## Rationale

- MariaDB:
	- Free open source license: GPL-2.0
	- [Receives active development mostly from MariaDB Corporation, Amazon, Codership, and independant contributors](https://mariadb.org/mariadb-11-0-3-10-11-5-10-10-6-10-9-8-10-6-15-10-5-22-10-4-31-now-available/).
	- Low-barrier-to-entry:
		- Easy to install and manage with open documentation.
		- Accessible on most operating systems (Windows + Linux).
		- Compatible with MySQL, Oracle SQL.
		- All features are available on the open-source community version.

[comment]: # "[MySQL Workbench](https://github.com/mysql/mysql-workbench)"
[comment]: # "[MySQLTuner](https://github.com/major/MySQLTuner-perl)"
[comment]: # "[mariadb-query-digest](https://mariadb-corporation.github.io/mariadb-tools/mariadb-query-digest.html)"

- Local/Self-Host:
	- Allows users to manage their own private information which ensure's the user's right to privacy, autonomy, and security.
	- Removes a responsibility/liability in terms of managing and securing cloud-hosted user data.

- Encrypted:
	- Provides a layer of safety for securing user data.

<br/>

## Consequences

Unknown Variables:
- We have to learn the nuances as we were primarily taught Oracle*SQL for our course.

MariaDB Limitations:
- Longterm Support:
	- 5 years for LTS versions: [10.4, 10.5, 10.6, 10.11](https://mariadb.org/download/)