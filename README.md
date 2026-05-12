# Kali Linux Foundation Building Problem-Solving
# Problem 1 - Find the Mail Server (MX Record) for google.com using dig/nslookup
Step by step command used - 
1. dig google.com MX [OR dig google.com MX +short]
2. Find the ANSWER SECTION
# Problem 2 - Route curl requests through Tor Network and verify identity rotation
Step by step command used -
1. sudo apt install tor [Click y/yes then]
2. sudo systemctl start tor
3. curl --socks5-hostname 127.0.0.1:9050 "https://icanhazip.com" "https://icanhazip.com"
4. sudo systemctl restart tor
5. curl --socks5-hostname 127.0.0.1:9050 "https://icanhazip.com" "https://icanhazip.com" [Again]
# Problem 3 - Write Bash Script to create 10 folders named YourName_1 through 10
Step by step command used -
1. nano make_folders.sh
2. [ONLY IN NANO TXT EDTIOR]
    #!/bin/bash
    for i in {1..10}
    do
    mkdir "YourName_$1"
   done
3. chmod +x make_folders.sh
4. ./make_folders.sh
5. ls [TO CHECK]
