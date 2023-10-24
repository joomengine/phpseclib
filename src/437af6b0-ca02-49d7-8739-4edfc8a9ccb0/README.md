```
██████╗  ██████╗ ██╗    ██╗███████╗██████╗
██╔══██╗██╔═══██╗██║    ██║██╔════╝██╔══██╗
██████╔╝██║   ██║██║ █╗ ██║█████╗  ██████╔╝
██╔═══╝ ██║   ██║██║███╗██║██╔══╝  ██╔══██╗
██║     ╚██████╔╝╚███╔███╔╝███████╗██║  ██║
╚═╝      ╚═════╝  ╚══╝╚══╝ ╚══════╝╚═╝  ╚═╝
```
# class Legacy (Details)
> namespace: **VDM\Joomla\Componentbuilder\Crypt\Aes**
```uml
@startuml
class Legacy  #Gold {
  # BASEAES $aes
  # int $size
  + __construct(BASEAES $aes)
  + encrypt(string $string, string $key) : string
  + decrypt(string $string, string $key) : ?string
}

note right of Legacy::__construct
  Constructor

  since: 3.2.0
end note

note right of Legacy::encrypt
  Encrypt a string as needed

  since: 3.2.0
  return: string
end note

note right of Legacy::decrypt
  Decrypt a string as needed

  since: 3.2.0
  return: ?string
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

