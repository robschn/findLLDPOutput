# findLLDPOutput
This will pull just the names from a "sh lldp nei". Please name your text file "input.txt"

Requires you to delete the "Capability codes", "Device ID" and "Total entries displayed", as well as add a space between the name and interface if needed.

Example:

Output of "sh lldp nei":

Capability codes:
    (R) Router, (B) Bridge, (T) Telephone, (C) DOCSIS Cable Device
    (W) WLAN Access Point, (P) Repeater, (S) Station, (O) Other

Device ID           Local Intf     Hold-time  Capability      Port ID
AP.431              Gi4/0/6        120        W               0000.0017.f028
AP.113SuperlongAPnamGi1/0/13       120        W               0000.0017.eee0
AP.320              Gi3/0/17       120        W               0000.0017.ec84
AP.108              Gi1/0/4        120        W               0000.0017.f4d0
AP.410              Gi3/0/32       120        W               0000.0017.f598
AP.309              Gi2/0/33       120        W               0000.0017.eccc
AP.220              Gi2/0/10       120        W               0000.0017.f050
AP.206              Gi1/0/31       120        W               0000.0017.ee4c

Total entries displayed: 8

Desired input for script:

AP.431              Gi4/0/6        120        W               0000.0017.f028
AP.113SuperlongAPnam Gi1/0/13       120        W               0000.0017.eee0
AP.320              Gi3/0/17       120        W               0000.0017.ec84
AP.108              Gi1/0/4        120        W               0000.0017.f4d0
AP.410              Gi3/0/32       120        W               0000.0017.f598
AP.309              Gi2/0/33       120        W               0000.0017.eccc
AP.220              Gi2/0/10       120        W               0000.0017.f050
AP.206              Gi1/0/31       120        W               0000.0017.ee4c
