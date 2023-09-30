# ConfigMate

ConfigMate is a utility for managing and storing configuration settings, usernames, passwords, and other key-value pairs in a convenient way. It allows you to easily write, read, edit, delete, and copy these key-value pairs

## Usage

```bash
configmate [-h] [-w <key> <value>] [-r <key>] [-d <key>] [-c <key>] [-l]
```

### Alternative

```bash
cfm [-h] [-w <key> <value>] [-r <key>] [-d <key>] [-c <key>] [-l]
```

### Options

- `-h`: Display the help message.
- `-w <key> <value>`: Write or edit a key with a value.
- `-r <key>`: Read a key's value.
- `-d <key>`: Delete the key and its value.
- `-c <key>`: Copy a key's value to the clipboard.
- `-l`: List all keys.

### Examples

1. Write or Edit a Key:
   ```bash
   configmate -w username john_doe
   cfm -w username john_doe
   ```

2. Read a Key's Value:
   ```bash
   configmate -r username
   cfm -r username
   ```

3. Delete a Key:
   ```bash
   configmate -d username
   cfm -d username
   ```

4. Copy a Key's Value to Clipboard:
   ```bash
   configmate -c username
   cfm -c username
   ```

5. List All Keys:
   ```bash
   configmate -l
   cfm -l
   ```

## Installation

- To install ConfigMate, simply run the following command:
   ```bash
   sudo dpkg -i configmate.deb
   ```

## Requirements

- `xclip` for copying values to the clipboard. Install it using your package manager if not already installed.

## Note

- The script uses a simple configuration file (`configmate.conf`) to store key-value pairs.
