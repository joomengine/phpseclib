```
██████╗  ██████╗ ██╗    ██╗███████╗██████╗
██╔══██╗██╔═══██╗██║    ██║██╔════╝██╔══██╗
██████╔╝██║   ██║██║ █╗ ██║█████╗  ██████╔╝
██╔═══╝ ██║   ██║██║███╗██║██╔══╝  ██╔══██╗
██║     ╚██████╔╝╚███╔███╔╝███████╗██║  ██║
╚═╝      ╚═════╝  ╚══╝╚══╝ ╚══════╝╚═╝  ╚═╝
```
# class Server (Details)
> namespace: **VDM\Joomla\Componentbuilder**
> extends: ****
```uml
@startuml
class Server  #Gold {
  # Load $load
  # Ftp $ftp
  # Sftp $sftp
  # User $user
  + __construct(Load $load, Ftp $ftp, ...)
  + move(int $id, string $localPath, ...) : bool
  + legacyMove(string $localPath, string $fileName, ...) : bool
}

note right of Server::__construct
  Constructor

  since: 3.2.0
  
  arguments:
    Load $load
    Ftp $ftp
    Sftp $sftp
    ?User $user = null
end note

note right of Server::move
  Move File to Server

  since: 3.2.0
  return: bool
  
  arguments:
    int $id
    string $localPath
    string $fileName
    ?int $protocol = null
    string $permission = 'core.export'
end note

note right of Server::legacyMove
  Move File to Server (Legacy Signature)

  since: 3.2.0
  return: bool
  
  arguments:
    string $localPath
    string $fileName
    int $serverID
    int $protocol = null
    string $permission = 'core.export'
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

