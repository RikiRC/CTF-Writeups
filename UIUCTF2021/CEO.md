# CEO
# Description:
You just wirelessly captured the handshake of the CEO of a multi-million dollar company! Use your password cracking skills to get the password! Wrap the password in the flag format. E.g: uiuctf{password}

# Solution:
- Download attached file and use aircrack-ng with rockyou password list
  - aircrack-ng -w rockyou.txt megacorp-01.cap
  - Link to the rockyou dictionary - https://github.com/brannondorsey/naive-hashcat/releases/download/data/rockyou.txt

# Flag:
uiuctf{nanotechnology}
