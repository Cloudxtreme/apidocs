## j.system.net

- /opt/jumpscale7/lib/JumpScale/core/system/net.py

### Methods

#### bridgeExists 
##### arguments

    - bridgename

##### comments

#### checkIpAddressIsLocal 
##### arguments

    - ipaddr

##### comments

#### checkListenPort 
##### arguments

    - port

##### comments

Check if a certain port is listening on the system.

@param port: sets the port number to check
@return status: 0 if running 1 if not running

#### checkUrlReachable 
##### arguments

    - url

##### comments

raise operational critical if unreachable
return True if reachable

#### download 
##### arguments

    - url
    - localpath
    - username
    - passwd

##### comments

Download a url to a file or a directory, supported protocols: http, https, ftp, file
@param url: URL to download from
@type url: string
@param localpath: filename or directory to download the url to pass - to return data
@type localpath: string
@param username: username for the url if it requires authentication
@type username: string
@param passwd: password for the url if it requires authentication
@type passwd: string

#### downloadIfNonExistent 
##### arguments

    - url
    - destination_file_path
    - md5_checksum
    - http_auth_username
    - http_auth_password

##### comments

Downloads the file from the specified url to the specified destination if it is not already there
or if the target file checksum doesn't match the expected checksum.

#### enableProxy 
##### arguments

##### comments

#### getDefaultIPConfig 
##### arguments

##### comments

#### getDefaultRouter 
##### arguments

##### comments

Get default router
@rtype: string representing the router interface

#### getDomainName 
##### arguments

##### comments

Retrieve the dns domain name

#### getHostByName 
##### arguments

    - dnsHostname

##### comments

#### getHostNamesForIP 
##### arguments

    - hostsfile
    - ip

##### comments

Get hostnames for ip address
@param hostsfile: File where hosts are defined
@param ip: Ip of the machine to get hostnames from
@return: List of machinehostnames

#### getHostname 
##### arguments

##### comments

Get hostname of the machine

#### getIpAddress 
##### arguments

    - interface

##### comments

Return a list of ip addresses and netmasks assigned to this interface

#### getIpAddresses 
##### arguments

    - up = False

##### comments

#### getMacAddress 
##### arguments

    - interface

##### comments

Return the MAC address of this interface

#### getMacAddressForIp 
##### arguments

    - ipaddress

##### comments

Search the MAC address of the given IP address in the ARP table

@param ipaddress: IP address of the machine
@rtype: string
@return: The MAC address corresponding with the given IP
@raise: RuntimeError if no MAC found for IP or if platform is not suppported

#### getNameServer 
##### arguments

##### comments

Returns the first nameserver IP found in /etc/resolv.conf

Only implemented for Unix based hosts.

@returns: Nameserver IP
@rtype: string

@raise NotImplementedError: Non-Unix systems
@raise RuntimeError: No nameserver could be found in /etc/resolv.conf

#### getNetworkInfo 
##### arguments

##### comments

returns \{macaddr_name:[ipaddr,ipaddr],...\}

REMARK: format changed because there was bug which could not work with bridges

@TODO change for windows

#### getNicType 
##### arguments

    - interface

##### comments

Get Nic Type on a certain interface
@param interface: Interface to determine Nic type on
@raise RuntimeError: On linux if ethtool is not present on the system

#### getNics 
##### arguments

    - up = False

##### comments

Get Nics on this machine
Works only for Linux/Solaris systems
@param up: only returning nics which or up

#### getReachableIpAddress 
##### arguments

    - ip
    - port

##### comments

Returns the first local ip address that can connect to the specified ip on the specified port

#### getVlanTag 
##### arguments

    - interface
    - nicType

##### comments

Get VLan tag on the specified interface and vlan type

#### getVlanTagFromInterface 
##### arguments

    - interface

##### comments

Get vlan tag from interface
@param interface: string interface to get vlan tag on
@rtype: integer representing the vlan tag

#### isIpInHostsFile 
##### arguments

    - hostsfile
    - ip

##### comments

Check if ip is in the hostsfile
@param hostsfile: File where hosts are defined
@param ip: Ip of the machine to check

#### isIpLocal 
##### arguments

    - ipaddress

##### comments

#### isNicConnected 
##### arguments

    - interface

##### comments

#### pingMachine 
##### arguments

    - ip
    - pingtimeout = 60
    - recheck = False
    - allowhostname = True

##### comments

Ping a machine to check if it's up/running and accessible
@param ip: Machine Ip Address
@param pingtimeout: time in sec after which ip will be declared as unreachable
@param recheck: Unused, kept for backwards compatibility
@param allowhostname: allow pinging on hostname (default is false)
@rtype: True if machine is pingable, False otherwise

#### pm_formatMacAddress 
##### arguments

    - macaddress

##### comments

#### removeFromHostsFile 
##### arguments

    - hostsfile
    - ip

##### comments

Update a hostfile, delete ip from hostsfile
@param hostsfile: File where hosts are defined
@param ip: Ip of the machine to remove

#### removeNetworkFromInterfaces 
##### arguments

    - network = '192.168.1'

##### comments

#### resetDefaultGateway 
##### arguments

    - gw

##### comments

#### setBasicNetConfiguration 
##### arguments

    - interface = 'eth0'
    - ipaddr
    - gw
    - mask = 24
    - config = True

##### comments

@param config if True then will be stored in linux configuration files

#### setBasicNetConfigurationBridgePub 
##### arguments

    - interface
    - ipaddr
    - gw
    - mask

##### comments

will in a safe way configure bridge brpub
if available and has ip addr to go to internet then nothing will happen
otherwise system will try in a safe way set this ipaddr, this is a dangerous operation

if ipaddr == None then will look for existing config on interface and use that one to configure the bridge

#### setBasicNetConfigurationDHCP 
##### arguments

    - interface = 'eth0'

##### comments

this will bring all bridges down

#### tcpPortConnectionTest 
##### arguments

    - ipaddr
    - port
    - timeout

##### comments

#### updateHostsFile 
##### arguments

    - hostsfile
    - ip
    - hostname

##### comments

Update a hostfile to contain the basic information install
@param hostsfile: File where hosts are defined
@param ip: Ip of the machine to add/modify
@param hostname: List of machinehostnames to add/modify

#### validateIpAddress 
##### arguments

    - ipaddress

##### comments

Validate wether this ip address is a valid ip address of 4 octets ranging from 0 to 255 or not
@param ipaddress: ip address to check on
@rtype: boolean...True if this ip is valid, False if not

#### waitConnectionTest 
##### arguments

    - ipaddr
    - port
    - timeout

##### comments

will return false if not successfull (timeout)

#### waitConnectionTestStopped 
##### arguments

    - ipaddr
    - port
    - timeout

##### comments

will test that port is not active
will return false if not successfull (timeout)

