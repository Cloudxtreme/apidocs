## j.servers.tornado

- /opt/jumpscale7/lib/JumpScale/grid/tornado/TornadoFactory.py

    #### def getClient(addr, port, category="core", org="myorg", user="root", passwd="passwd", ssl=False, roles=[]) 
    #### def getHAClient(connections, category="core", org="myorg", user="root", passwd="passwd", ssl=False, roles=[],id=None,timeout=60, reconnect=False) 
    #### def getServer(port, sslorg=None, ssluser=None, sslkeyvaluestor=None) 
    
    HOW TO USE:
    daemon=j.servers.tornado.getServer(port=4444)
    
    class MyCommands():
        def __init__(self,daemon):
            self.daemon=daemon
    
        #session always needs to be there
        def pingcmd(self,session=session):
            return "pong"
    
        def echo(self,msg="",session=session):
            return msg
    
    daemon.addCMDsInterface(MyCommands,category="optional")  #pass as class not as object !!! chose category if only 1 then can leave ""
    
    daemon.start()
    #### def initSSL4Server(organization, serveruser, sslkeyvaluestor=None) 
    
    use this to init your ssl keys for the server (they can be used over all transports)
