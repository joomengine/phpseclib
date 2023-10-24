```
██████╗  ██████╗ ██╗    ██╗███████╗██████╗
██╔══██╗██╔═══██╗██║    ██║██╔════╝██╔══██╗
██████╔╝██║   ██║██║ █╗ ██║█████╗  ██████╔╝
██╔═══╝ ██║   ██║██║███╗██║██╔══╝  ██╔══██╗
██║     ╚██████╔╝╚███╔███╔╝███████╗██║  ██║
╚═╝      ╚═════╝  ╚══╝╚══╝ ╚══════╝╚═╝  ╚═╝
```
# class Aes (Details)
> namespace: **VDM\Joomla\Componentbuilder\Crypt**
```uml
@startuml
class Aes  #Gold {
  # BASEAES $aes
  # Random $random
  # int $size
  + __construct(BASEAES $aes, Random $random)
  + encrypt(string $string, string $key) : string
  + decrypt(string $string, string $key) : ?string
}

note right of Aes::__construct
  Constructor

  since: 3.2.0
end note

note right of Aes::encrypt
  Encrypt a string as needed

  since: 3.2.0
  return: string
end note

note right of Aes::decrypt
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

