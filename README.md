# Linux Script to Back Up Folders Using a Config File

## Description

A simple Bash script that backs up folders using a JSON config file. 

Requires jq to parse the config. 

Archives folders as timestamped .tar.gz files. 

Supports multiple backup tasks.

## Usage

1. **Download the repository:**
   - [Download ZIP](https://github.com/shatakratu/bash-backup-script/archive/refs/heads/main.zip)

2. **Install jq to parse JSON:**
   ```bash
   sudo apt install jq
   ```

3. **Edit the config file** (`backup_config.json`):

   - `"backup_name"`   – name of the archive to be created
   - `"source_folder"` – path to the folder you want to back up
   - `"target_folder"` – path where the archive will be saved

4. **Make the script executable:**
   ```bash
   chmod +x backup_script.sh
   ```

5. **Run the script:**
   ```bash
   ./backup_script.sh
   ```