# check_sap_longrunningjobs_utc.py
Nagios plugin for checking SAP long running jobs

![](/images/check_sap_longrunningjobs_utc2.png)

![](/images/check_sap_longrunningjobs_utc.png)


Usage:./check_sap_longrunningjobs_utc.py \<SID\> \<seconds\> 

Example:

root@h:~/github# ./check_sap_longrunningjobs_utc.py SBX 1000

CRITICAL - 7 Jobs running over 1000 seconds | jobs=7


                                                                      
### Prerequisite:
https://github.com/piersharding/python-sapnwrfc

### Wiki:
Installation of sapnwrfc for python on Linux and Unix
https://wiki.scn.sap.com/wiki/display/EmTech/Installation+of+sapnwrfc+for+python+on+Linux+and+Unix






To prepare a script, you'll need a 'yml' file similar to the 'sap.yml' file included with the sapnwrfc download. The file looks 

like this:
#### Example of SID.yml file

ashost: gecko.local.net

sysnr: "01"

client: "001"

user: developer

passwd: developer

lang: EN

trace: 3

loglevel: warn
