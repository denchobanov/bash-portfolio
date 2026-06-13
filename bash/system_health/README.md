# System Health Monitor

A lightweight, automated Bash script designed to monitor system resource usage (CPU, RAM, Disk) and provide real-time alerts. Ideal for system administrators who need a quick health check or an automated reporting tool for server maintenance.

## Features
- **Automated Metrics:** Monitors CPU, RAM, and Disk usage in real-time.
- **Threshold Alerts:** Issues warnings if any resource usage exceeds the defined 80% threshold.
- **Non-Interactive:** Designed to run via `cron` jobs without requiring user input.
- **Logging:** Saves all health reports to a dedicated log file.
- **Backup:** Automatically creates a timestamped backup of the current health status.

## Usage

### Prerequisites
- Linux-based system
- `bash`, `awk`, `top`, `free`, `df`

### Running the script
You can run the script manually by specifying a destination folder for the logs:

```bash
./system_health.sh /path/to/your/logs
