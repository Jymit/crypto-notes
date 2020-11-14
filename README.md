# getschwifty













Reverse Engineering Crypto







XOR



RC4 Crypto
https://en.wikipedia.org/wiki/RC4
Key-scheduling algorithm (KSA)
```
for i from 0 to 255
    S[i] := i
endfor
j := 0
for i from 0 to 255
    j := (j + S[i] + key[i mod keylength]) mod 256
    swap values of S[i] and S[j]
endfor
```
S box init of 255 array. while loop. mod key length so as to not go past 255.







Tools
https://ghidra-sre.org/releaseNotes_9.2.html - inc decompiler
https://www.hex-rays.com/products/ida/support/download_freeware/IDA - supports some architectures that Ghidra doesn't, and vice versa. IDA has a debugger whereas Ghidra does not.
https://gchq.github.io/CyberChef/ - live web based decrytion for testing once key, data, data length and input format is entered.
https://www.hopperapp.com/ - 
https://docs.pwntools.com/en/stable/about.html - for python crypto decryption testing once data pulled out of disassem

Ghidra
run to get to entry point
G to go to addr
function graph and function call graph

Hopper
open binary > procs > main
Alt + Enter to decomp
G to go to addr



CrackMes
