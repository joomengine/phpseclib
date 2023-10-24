```
██████╗  ██████╗ ██╗    ██╗███████╗██████╗
██╔══██╗██╔═══██╗██║    ██║██╔════╝██╔══██╗
██████╔╝██║   ██║██║ █╗ ██║█████╗  ██████╔╝
██╔═══╝ ██║   ██║██║███╗██║██╔══╝  ██╔══██╗
██║     ╚██████╔╝╚███╔███╔╝███████╗██║  ██║
╚═╝      ╚═════╝  ╚══╝╚══╝ ╚══════╝╚═╝  ╚═╝
```
# class Crypt (Details)
> namespace: **VDM\Joomla\Componentbuilder**
```uml
@startuml
class Crypt  #Gold {
  # FOF $fof
  # Aes $aes
  # Legacy $legacy
  # Password $password
  # array $options
  # array $passwords
  + __construct(FOF $fof, Aes $aes, ...)
  + encrypt(string $string, string $method, ...) : string
  + decrypt(string $string, string $method, ...) : ?string
  + exist(string $method) : bool
  - getClassName(string $method) : ?string
  - getClassNameFromRegistry(string $method) : ?string
  - getClassNameFromOptions(string $method) : ?string
  - getPassword(string $method, ?string $password = null) : ?string
  - getPasswordKey(string $method) : string
  - name(string $method) : string
}

note right of Crypt::__construct
  Constructor

  since: 3.2.0
  
  arguments:
    FOF $fof
    Aes $aes
    Legacy $legacy
    Password $password
end note

note left of Crypt::encrypt
  Encrypt a string as needed

  since: 3.2.0
  return: string
  
  arguments:
    string $string
    string $method
    ?string $password = null
end note

note right of Crypt::decrypt
  Decrypt a string as needed

  since: 3.2.0
  return: ?string
  
  arguments:
    string $string
    string $method
    ?string $default = null
end note

note left of Crypt::exist
  Check if a decryption method exist and is supported

  since: 3.2.0
  return: bool
end note

note right of Crypt::getClassName
  Get crypto class name to use

  since: 3.2.0
  return: ?string
end note

note left of Crypt::getClassNameFromRegistry
  Get the crypto class name from the registry

  since: 3.2.0
  return: ?string
end note

note right of Crypt::getClassNameFromOptions
  Get the crypto class name for the given encryption method and options

  since: 3.2.0
  return: ?string
end note

note left of Crypt::getPassword
  Get the password

  since: 3.2.0
  return: ?string
end note

note right of Crypt::getPasswordKey
  Get the key

  since: 3.2.0
  return: string
end note

note left of Crypt::name
  Get the class name

  since: 3.2.0
  return: string
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

