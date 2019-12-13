dubbo-remoting
     
    dubbo的远程通信模块，提供通用的客户端和服务端的通讯功能
        server
        client
        
dubbo-remoting-zookeepeer相当于是ZookeeperClient，和ZookeeperServer进行通信

dubbo-remoting-api，定义了DubboClient和DubboServer接口

    dubbo-remoting-grizzy，相当于是接口的Grizzy实现
    dubbo-remoting-http，基于netty和Tomcat实现
    dubbo-remoting-mina，是指接口基于mina实现
    dubbo-remoting-netty 是指基于Netty3实现
    dubbo—remoting-netty4 是指基于netty4实现
    dubbo-remoting-P2P 是dubbo的p2p服务器，注册中心dubbo-registry-multicast项目使用该项目
    
    从最小化程度看，我们只需要看dubbo-remoting-api + dubbo-remoting-netty + dubbo-remoting-zookeepeer


    
   