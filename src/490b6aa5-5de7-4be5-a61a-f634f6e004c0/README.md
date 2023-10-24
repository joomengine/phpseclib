```
██████╗  ██████╗ ██╗    ██╗███████╗██████╗
██╔══██╗██╔═══██╗██║    ██║██╔════╝██╔══██╗
██████╔╝██║   ██║██║ █╗ ██║█████╗  ██████╔╝
██╔═══╝ ██║   ██║██║███╗██║██╔══╝  ██╔══██╗
██║     ╚██████╔╝╚███╔███╔╝███████╗██║  ██║
╚═╝      ╚═════╝  ╚══╝╚══╝ ╚══════╝╚═╝  ╚═╝
```
# class Sftp (Details)
> namespace: **VDM\Joomla\Componentbuilder\Server**
```uml
@startuml
class Sftp  #Gold {
  # KeyLoader $key
  # ?SftpClient $client
  # ?object $details
  # CMSApplication $app
  + __construct(KeyLoader $key, ?CMSApplication $app = null)
  + set(object $details) : Sftp
  + move(string $localPath, string $fileName) : bool
  - connected() : bool
  - getClient() : ?SftpClient
}

note right of Sftp::__construct
  Constructor

  since: 3.2.0
end note

note right of Sftp::set
  set the server details

  since: 3.2.0
  return: Sftp
end note

note right of Sftp::move
  move a file to server with the FTP client

  since: 3.2.0
  return: bool
end note

note right of Sftp::connected
  Make sure we are connected

  since: 3.2.0
  return: bool
end note

note right of Sftp::getClient
  get the SftpClient object

  since: 3.2.0
  return: ?SftpClient
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

