```
██████╗  ██████╗ ██╗    ██╗███████╗██████╗
██╔══██╗██╔═══██╗██║    ██║██╔════╝██╔══██╗
██████╔╝██║   ██║██║ █╗ ██║█████╗  ██████╔╝
██╔═══╝ ██║   ██║██║███╗██║██╔══╝  ██╔══██╗
██║     ╚██████╔╝╚███╔███╔╝███████╗██║  ██║
╚═╝      ╚═════╝  ╚══╝╚══╝ ╚══════╝╚═╝  ╚═╝
```
# class FOF (Details)
> namespace: **VDM\Joomla\Componentbuilder\Crypt**
```uml
@startuml
class FOF  #Gold {
  # AES $aes
  # Random $random
  # int $size
  + __construct(AES $aes, Random $random)
  + encrypt(string $string, string $key) : string
  + decrypt(string $string, string $key) : string
  # getExpandedKey(string $key, int $blockSize, ...) : string
  # resizeKey(string $key, int $size) : ?string
}

note right of FOF::__construct
  Constructor

  since: 3.2.0
end note

note right of FOF::encrypt
  Encrypt a string as needed

  since: 3.2.0
  return: string
end note

note right of FOF::decrypt
  Decrypt a string as needed

  since: 3.2.0
  return: string
end note

note right of FOF::getExpandedKey
  Function taken from FOFEncryptAes
changed a little but basically the same
to ensure we get the same passwords (not ideal)
we should use `$this->aes->setPassword(...)` instead
but can't for backwards compatibility issues with already encrypted string

  since: 3.2.0
  return: string
  
  arguments:
    string $key
    int $blockSize
    string $iv
end note

note right of FOF::resizeKey
  Function taken from FOFEncryptAes
changed a little but basically the same
to ensure we get the same passwords (not ideal)
we should use `$this->aes->setPassword(...)` instead
but can't for backwards compatibility issues with already encrypted string

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

