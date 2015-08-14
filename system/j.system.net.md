## j.system.net

- /opt/jumpscale7/lib/JumpScale/core/system/net.py

### def getReachableIpAddress(ip, port) (l424)

Returns the first local ip address that can connect to the specified ip on the specified port

### def getDomainName() (l1171)

Retrieve the dns domain name

### def getVlanTag(interface,nicType=None) (l370)

Get VLan tag on the specified interface and vlan type

### def tcpPortConnectionTest(ipaddr,port, timeout=None) (l37)

### def setBasicNetConfigurationBridgePub(interface=None,ipaddr=None,gw=None,mask=None) (l596)

will in a safe way configure bridge brpub
if available and has ip addr to go to internet then nothing will happen
otherwise system will try in a safe way set this ipaddr, this is a dangerous operation

if ipaddr == None then will look for existing config on interface and use that one to configure the bridge

### def pm_formatMacAddress(macaddress) (l824)

### def getVlanTagFromInterface(interface) (l393)

Get vlan tag from interface
@param interface: string interface to get vlan tag on
@rtype: integer representing the vlan tag

### def download(url, localpath, username=None, passwd=None) (l1118)

Download a url to a file or a directory, supported protocols: http, https, ftp, file
@param url: URL to download from
@type url: string
@param localpath: filename or directory to download the url to pass - to return data
@type localpath: string
@param username: username for the url if it requires authentication
@type username: string
@param passwd: password for the url if it requires authentication
@type passwd: string

### def getHostname() (l896)

Get hostname of the machine

### def getHostNamesForIP(hostsfile, ip) (l1050)

Get hostnames for ip address
@param hostsfile: File where hosts are defined
@param ip: Ip of the machine to get hostnames from
@return: List of machinehostnames

### def getMacAddress(interface) (l787)

Return the MAC address of this interface

### def getNicType(interface) (l299)

Get Nic Type on a certain interface
@param interface: Interface to determine Nic type on
@raise RuntimeError: On linux if ethtool is not present on the system

### def getIpAddress(interface) (l736)

Return a list of ip addresses and netmasks assigned to this interface

### def enableProxy() (l245)

### def getNameServer() (l194)

Returns the first nameserver IP found in /etc/resolv.conf

Only implemented for Unix based hosts.

@returns: Nameserver IP
@rtype: string

@raise NotImplementedError: Non-Unix systems
@raise RuntimeError: No nameserver could be found in /etc/resolv.conf

### def setBasicNetConfigurationDHCP(interface="eth0") (l546)

this will bring all bridges down

### def isIpInHostsFile(hostsfile, ip) (l1022)

Check if ip is in the hostsfile
@param hostsfile: File where hosts are defined
@param ip: Ip of the machine to check

### def waitConnectionTest(ipaddr,port,timeout) (l52)

will return false if not successfull (timeout)

### def getDefaultRouter() (l936)

Get default router
@rtype: string representing the router interface

### def resetDefaultGateway(gw) (l450)

### def removeFromHostsFile(hostsfile, ip) (l1035)

Update a hostfile, delete ip from hostsfile
@param hostsfile: File where hosts are defined
@param ip: Ip of the machine to remove

### def validateIpAddress(ipaddress) (l951)

Validate wether this ip address is a valid ip address of 4 octets ranging from 0 to 255 or not
@param ipaddress: ip address to check on
@rtype: boolean...True if this ip is valid, False if not

### def waitConnectionTestStopped(ipaddr,port,timeout) (l71)

will test that port is not active
will return false if not successfull (timeout)

### def getNics(up=False) (l266)

Get Nics on this machine
Works only for Linux/Solaris systems
@param up: only returning nics which or up

### def bridgeExists(bridgename) (l442)

### def checkListenPort(port) (l110)

Check if a certain port is listening on the system.

@param port: sets the port number to check
@return status: 0 if running 1 if not running

### def setBasicNetConfiguration(interface="eth0",ipaddr=None,gw=None,mask=24,config=True) (l476)

@param config if True then will be stored in linux configuration files

### def isIpLocal(ipaddress) (l834)

### def getNetworkInfo() (l710)

returns \{macaddr_name:[ipaddr,ipaddr],...\}

REMARK: format changed because there was bug which could not work with bridges

@TODO change for windows

### def getMacAddressForIp(ipaddress) (l839)

Search the MAC address of the given IP address in the ARP table

@param ipaddress: IP address of the machine
@rtype: string
@return: The MAC address corresponding with the given IP
@raise: RuntimeError if no MAC found for IP or if platform is not suppported

### def pingMachine(ip, pingtimeout=60, recheck = False, allowhostname = True) (l980)

Ping a machine to check if it's up/running and accessible
@param ip: Machine Ip Address
@param pingtimeout: time in sec after which ip will be declared as unreachable
@param recheck: Unused, kept for backwards compatibility
@param allowhostname: allow pinging on hostname (default is false)
@rtype: True if machine is pingable, False otherwise

### def updateHostsFile(hostsfile,ip,hostname) (l1067)

Update a hostfile to contain the basic information install
@param hostsfile: File where hosts are defined
@param ip: Ip of the machine to add/modify
@param hostname: List of machinehostnames to add/modify

### def getIpAddresses(up=False) (l224)

### def removeNetworkFromInterfaces(network="192.168.1") (l536)

### def checkIpAddressIsLocal(ipaddr) (l239)

### def checkUrlReachable(url) (l88)

raise operational critical if unreachable
return True if reachable

### def downloadIfNonExistent(url, destination_file_path, md5_checksum=None, (l1089)

Downloads the file from the specified url to the specified destination if it is not already there
or if the target file checksum doesn't match the expected checksum.

### def getDefaultIPConfig() (l434)

### def getHostByName(dnsHostname) (l933)

### def isNicConnected(interface) (l901)

