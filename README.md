
# Linux Script to Back Up Folders Using a Config File

## Description

A simple Bash script to back up folders using a JSON configuration file.

The script uses `jq` to read the config file, so ensure `jq` is installed.

Each folder is saved as a `.tar.gz` archive with a timestamp.

## Usage

1. **Download the repository:**
   - [Download ZIP](https://github.com/shatakratu/bash-backup-script/archive/refs/heads/main.zip)

2. **Install required tool** (`jq` to parse JSON):
   ```bash
   sudo apt install jq
   ```

3. **Edit the configuration file** (`backup_config.json`):
   - `"backup_name"`: name of the archive to be created
   - `"source_folder"`: path to the folder to back up
   - `"target_folder"`: path where the archive will be saved

4. **Make the script executable:**
   ```bash
   chmod +x backup_script.sh
   ```

5. **Run the script:**
   ```bash
   ./backup_script.sh
   ```