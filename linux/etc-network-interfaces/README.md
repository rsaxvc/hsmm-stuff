Setting up BBHN with /etc/network/interfaces
====================

IP Calculation
---------------------
Please see higher lever article including this

Interface Setup
---------------------
To bind a single interface into ad-hoc
wifi mode for BBHN, put the following
into /etc/network/interfaces, or a
seperate file under /etc/network/interfaces.d/bbhn

    auto networkInterfaceLikeWlan0
    iface networkInterfaceLikeWlan0 inet static
            address 10.IP.AddrGoes.RightHere
            netmask 255.255.255.0
            wireless-channel 1
            wireless-essid BroadbandHamnet-v1
            wireless-mode ad-hoc
