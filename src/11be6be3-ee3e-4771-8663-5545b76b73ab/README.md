```
██████╗  ██████╗ ██╗    ██╗███████╗██████╗
██╔══██╗██╔═══██╗██║    ██║██╔════╝██╔══██╗
██████╔╝██║   ██║██║ █╗ ██║█████╗  ██████╔╝
██╔═══╝ ██║   ██║██║███╗██║██╔══╝  ██╔══██╗
██║     ╚██████╔╝╚███╔███╔╝███████╗██║  ██║
╚═╝      ╚═════╝  ╚══╝╚══╝ ╚══════╝╚═╝  ╚═╝
```
# class Ftp (Details)
> namespace: **VDM\Joomla\Componentbuilder\Server**
```uml
@startuml
class Ftp  #Gold {
  # ?FtpClient $client
  # ?object $details
  + set(object $details) : Ftp
  + move(string $localPath, string $fileName) : bool
  - connected() : bool
  - getClient() : ?FtpClient
}

note right of Ftp::set
  set the server details

  since: 3.2.0
  return: Ftp
end note

note right of Ftp::move
  move a file to server with the FTP client

  since: 3.2.0
  return: bool
end note

note right of Ftp::connected
  Make sure we are connected

  since: 3.2.0
  return: bool
end note

note right of Ftp::getClient
  get the FtpClient object

  since: 3.2.0
  return: ?FtpClient
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

