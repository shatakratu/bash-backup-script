# Linux Script to Back Up Folders Using a Config File

## Description

A simple Bash script to back up folders using a JSON configuration file.  

The script uses `jq` to read the config file, so make sure it’s installed.

## Usage

1. **Download the Backup Script:**  

   [zip](https://github.com/shatakratu/bash-backup-script/archive/refs/heads/main.zip)


2. **Install the Required Dependency (`jq`):**
   ```bash
   sudo apt install jq
   ```

3. **Edit the Configuration File (`backup_config.json`)**

   Example:
```json
{
  "backup_name": "project_backup",
  "source_folder": "/home/user/project",
  "target_folder": "/home/user/backups"
}
```
- backup_name — name of your backup archive
- source_folder — full path to the folder you want to back up
- target_folder — full path to the folder where the archive should be saved  
&nbsp;

4. **Make the Script Executable:**
   ```bash
   chmod +x backup_script.sh
   ```

5. **Run the Script:**
   ```bash
   ./backup_script.sh
   ```