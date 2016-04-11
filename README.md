# aqua

Installation for Debian:

    Install dependencies -
        "su"
        "apt install python3-flask zlib1g-dev gcc make git autoconf autogen automake pkg-config" 
        "exit"

    Install netdata -
        "su"
        "cd && mkdir nd && cd nd"
        "git clone https://github.com/firehol/netdata.git --depth=1"
        "cd netdata"
        "./netdata-installer.sh"
        "exit"

    Then run it -
        "su"
        "/usr/sbin/netdata"
        "exit"
    
    If you want it to run at every boot - 
        "su"
        "nano /etc/rc.local"
        Append "/usr/sbin/netdata" before the exit
        Ctrl-X, Y, Enter

    Now you can run with
        ./server.py
