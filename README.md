# ADBash - Your Local ADB Shell for Termux

## About

**ADBash** is a small Bash script made specifically for Termux on Android.  
It connects Termux to the ADB host running on the same device (localhost / 127.0.0.1) and launches a full Bash session inside it.  
The script is fully automated, minimal, and requires only a few basic tools to work.

![screenshot](/screenshot.jpg)

## Features

- Connects Termux directly to the Android ADB host on localhost
- Opens a ready-to-use Bash shell inside the ADB session
- Automatically detects the local ADB port
- Works without root access
- Pure Bash with minimal dependencies
- Includes quick help and basic info screens
- Clean and simple design focused on automation
- Compatible with Android 10+ and Termux environments

## Installation

Clone the repository and make the script executable:

### ADBash script

```bash
git clone https://github.com/BuriXon-code/ADBash
cd ADBash
chmod +x ADBash.sh
```

### Dependencies

Install required packages in Termux:

```bash
pkg update
pkg install nmap
pkg install android-tools
```

That’s all you need to run ADBash.

### Wireless Debugging on Android 10+

Starting from Android 10, ADB connections over Wi-Fi require manual pairing with a PIN.

This must be done once before using ADBash:

1. Enable Developer options  
2. Enable Wireless debugging  
3. Pair device with pairing code  
4. Use the IP, port, and PIN shown on your phone to complete pairing  

Once your Termux is authorized, ADBash can connect automatically in future sessions.
A short video demonstrating ADB pairing on my device running Android 15 can be found [here](https://burixon.dev/projects/ADBash/).

> [!WARNING]
> Without prior ADB pairing, the script will not work. This is a mandatory step that cannot really be automated.

## Usage

Run the script without arguments to start a connection and open an ADBash session:

```bash
./ADBash.sh
```

### Options

- `-v`, `--verbose` - enable verbose output
- `-n`, `--nobash` - run ADB shell without starting Bash
- `-r`, `--rcfile` - use a custom Bash rc file
- `-p`, `--port` - manualy set ADB port
- `-s`, `--scan-port` - scan for available ADB ports only
- `-h`, `--help` - show minimal help
- `-C`, `--codes` - show exit codes and their meaning
- `-A`, `--about` - show author and script information
- `-V`, `--version` - show version information

### Examples

Start normally:
```bash
./ADBash.sh
```

Run with custom rc file:
```bash
./ADBash.sh -r /sdcard/customrc
```

Scan for ADB port only:
```bash
./ADBash.sh -s
```

Show exit codes:
```bash
./ADBash.sh -C
```

Show about info:
```bash
./ADBash.sh -A
```

### Help

1. Help option
```bash
./ADBash.sh -h
```
The `-h` `--help` option displays general information about the parameters and options accepted by the script.

2. About option
```bash
./ADBash.sh -A
```
The `-A` `--about` option provides information about the author, legal details, a brief description of the script, and information about its purpose.

3. Codes option
```bash
./ADBash.sh -C
```
The `-C` `--codes` option provides full information about the types and meanings of error codes returned by the script.
> By default, the script displays minimal output and information (for aesthetics and a 'wow' effect), so these codes are the primary way of indicating the operation status.  

## Dependencies

- `bash` - main interpreter  
- `nmap` - used to detect open ADB ports  
- android-tools (`adb`) - required for ADB shell sessions  
- Android 10+ - for Wireless Debugging and pairing support  
- no root required  
- network pairing required once for local ADB communication  

## License

ADBash is released under the **GNU General Public License v3.0 (GPLv3)**.  
You can use, modify, and share it freely under the same license.  
Commercial use or relicensing under a closed-source license is not allowed.  
See the LICENSE file for full terms.

## Support
### Contact me:
For any issues, suggestions, or questions, reach out via:

- *Email:* support@burixon.dev  
- *Contact form:* [Click here](https://burixon.dev/contact/)
- *Bug reports:* [Click here](https://burixon.dev/bugreport/#ADBash)

> [!NOTE]
> Pairing the device with the ADB daemon is a fundamental step; unfortunately, this process varies across devices depending on the Android version and system overlay. Therefore, I will not answer messages regarding device pairing with ADB!  

### Support me:
If you find this script useful, consider supporting my work by making a donation:

[**Donations**](https://burixon.dev/donate/)

Your contributions help in developing new projects and improving existing tools!
