# Log-Archive-Tool
## Project URL  
[project URL](https://roadmap.sh/projects/log-archive-tool) 


A Python-based tool to archive logs, compress them, and keep your system organized by storing them in a compressed format for future reference.

## Overview
This tool archives logs from directories like `/var/log` (commonly used for system and application logs on Unix-based systems), compresses them into a `.tar.gz` file, and logs the archive activity.

---

## Steps to Use the Tool

### 1. Create the Python Script
Create the `log-archive.py` file:
```bash
vim log-archive.py
```


markdown
Copy code
# Log-Archive-Tool

A Python-based tool to archive logs, compress them, and keep your system organized by storing them in a compressed format for future reference.

## Overview
This tool archives logs from directories like `/var/log` (commonly used for system and application logs on Unix-based systems), compresses them into a `.tar.gz` file, and logs the archive activity.

---

## Steps to Use the Tool

### 1. Create the Python Script
Create the `log-archive.py` file:
```bash
vim log-archive.py
```
## Add the Python code to archive logs.

### 2. Run the Script
## Run the following command to compress logs in /var/log:

```bash
sudo python log-archive.py /var/log
```
## Note: The /var/log directory requires root permissions to modify.



### 3. Success Message
## After running the script, you’ll see a message like this:

```
Logs successfully archived to /var/log/archived_logs/logs_archive_20241127_143425.tar.gz
```

### 4. View Archive Contents
## To see the files inside the .tar.gz archive, use:

```bash
tar -tzvf /var/log/archived_logs/logs_archive_20241127_143425.tar.gz
```

### About /var/log
The /var/log directory stores logs generated by the operating system, services, and applications. Examples include:

 System Logs: syslog, dmesg
 Authentication Logs: auth.log
 Service Logs: nginx/, apache2/
