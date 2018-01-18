- Compatible devices
 
       Aruba:    generic
       Brocade:  generic
       D-link:   DES-3226S
                 DES-3526
                 DGS-1510
                 DGS-3100
                 DGS-3120
        HP:      1910
                 2620
                 2640
                 2910
                 A5120
       Huawei:   S5700
                 CE6810
       3Com:     3226
                 4500
                 4800
                 7750A
        Netgear: GS724T

- Getting Started

Installing a TFTP serer on Debian flavors:

    $ sudo apt-get install tftpd-hpa
  
Set params to TFTP service:
  
    $ sudo vi /etc/default/tftpd-hpa

Change address and path dir:

    TFTP_USERNAME="tftp"
    TFTP_DIRECTORY="/path/to/bkp/files"
    TFTP_ADDRESS="0.0.0.0:69"
    TFTP_OPTIONS="--secure"
