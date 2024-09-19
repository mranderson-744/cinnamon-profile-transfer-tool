# Cinnamon Profile Transfer Tool

## Overview
This script allows you to easily copy and transfer Cinnamon desktop configurations, themes, icons, and start menu icon settings from one user to another in a Linux environment.

## Features
- Export and import Cinnamon settings using `dconf`.
- Copy GTK, icon, and shell themes from the source user.
- Handle start menu icon configuration by copying the appropriate JSON file.
- Handles permission issues by utilizing `sudo` where necessary.

## Requirements
- **Linux with Cinnamon desktop**: The script is designed for systems running the Cinnamon desktop environment.
- **`dconf` utility**: The script uses `dconf` to manage settings.
- **`sudo` privileges**: You may need administrative rights to run certain commands.

## Usage
1. Log in to target linux user
2. git clone https://github.com/mranderson-744/cinnamon-profile-transfer-tool.git && cd cinnamon-profile-transfer-tool
3. Make the script executable:
   ```bash
   chmod +x pull_cinnamon_profile_from
   ```
4. Run the script, specifying the username of the source user:
   ```bash
   ./pull_cinnamon_profile_from <username>
   ```
5. Enjoy your configs applied!

## Example
To copy the Cinnamon profile from user `mainuser` to the currently logged-in user `targetuser`, run:
```bash
./pull_cinnamon_profile_from mainuser 
```

## Contributing
Feel free to submit issues or pull requests if you have suggestions for improvements or find bugs.

## License
This project is licensed under the MIT License.

