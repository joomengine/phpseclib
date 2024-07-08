```
██████╗  ██████╗ ██╗    ██╗███████╗██████╗
██╔══██╗██╔═══██╗██║    ██║██╔════╝██╔══██╗
██████╔╝██║   ██║██║ █╗ ██║█████╗  ██████╔╝
██╔═══╝ ██║   ██║██║███╗██║██╔══╝  ██╔══██╗
██║     ╚██████╔╝╚███╔███╔╝███████╗██║  ██║
╚═╝      ╚═════╝  ╚══╝╚══╝ ╚══════╝╚═╝  ╚═╝
```
# class Server (Details)
> namespace: **VDM\Joomla\Componentbuilder\Service**
> extends: ****
```uml
@startuml
class Server  #Gold {
  + register(Container $container) : void
  + getServer(Container $container) : Client
  + getServerLoad(Container $container) : Load
  + getServerFtp(Container $container) : Ftp
  + getServerSftp(Container $container) : Sftp
}

note right of Server::register
  Registers the service provider with a DI container.

  since: 3.2.0
  return: void
end note

note right of Server::getServer
  Get the Server Client class

  since: 3.2.0
  return: Client
end note

note right of Server::getServerLoad
  Get the Server Load class

  since: 3.2.0
  return: Load
end note

note right of Server::getServerFtp
  Get the Server Ftp class

  since: 3.2.0
  return: Ftp
end note

note right of Server::getServerSftp
  Get the Server Sftp class

  since: 3.2.0
  return: Sftp
end note
 
@enduml
```

---
```
     ██╗ ██████╗██████╗
     ██║██╔════╝██╔══██╗
     ██║██║     ██████╔╝
██   ██║██║     ██╔══██╗
╚█████╔╝╚██████╗██████╔╝
 ╚════╝  ╚═════╝╚═════╝
```
> Build with [Joomla Component Builder](https://git.vdm.dev/joomla/Component-Builder)

