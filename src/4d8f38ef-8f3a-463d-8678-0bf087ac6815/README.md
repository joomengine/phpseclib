```
██████╗  ██████╗ ██╗    ██╗███████╗██████╗
██╔══██╗██╔═══██╗██║    ██║██╔════╝██╔══██╗
██████╔╝██║   ██║██║ █╗ ██║█████╗  ██████╔╝
██╔═══╝ ██║   ██║██║███╗██║██╔══╝  ██╔══██╗
██║     ╚██████╔╝╚███╔███╔╝███████╗██║  ██║
╚═╝      ╚═════╝  ╚══╝╚══╝ ╚══════╝╚═╝  ╚═╝
```
# class Crypt (Details)
> namespace: **VDM\Joomla\Componentbuilder\Service**
> extends: ****
```uml
@startuml
class Crypt  #Gold {
  + register(Container $container) : void
  + getCrypt(Container $container) : Crypto
  + getPassword(Container $container) : Password
  + getRandom(Container $container) : Random
  + getKeyLoader(Container $container) : KeyLoader
  + getBASEAESCBC(Container $container) : BASEAES
  + getAesCBC(Container $container) : Aes
  + getAesLEGACY(Container $container) : Legacy
  + getFOF(Container $container) : FOF
}

note right of Crypt::register
  Registers the service provider with a DI container.

  since: 3.2.0
  return: void
end note

note left of Crypt::getCrypt
  Get the Crypto class

  since: 3.2.0
  return: Crypto
end note

note right of Crypt::getPassword
  Get the Password class

  since: 3.2.0
  return: Password
end note

note left of Crypt::getRandom
  Get the Random class

  since: 3.2.0
  return: Random
end note

note right of Crypt::getKeyLoader
  Get the KeyLoader class

  since: 3.2.0
  return: KeyLoader
end note

note left of Crypt::getBASEAESCBC
  Get the AES Cyper with CBC mode

  since: 3.2.0
  return: BASEAES
end note

note right of Crypt::getAesCBC
  Get the Wrapper AES Cyper with CBC mode

  since: 3.2.0
  return: Aes
end note

note left of Crypt::getAesLEGACY
  Get the Wrapper AES Legacy Cyper with CBC mode

  since: 3.2.0
  return: Legacy
end note

note right of Crypt::getFOF
  Get the FOF AES Cyper with CBC mode

  since: 3.2.0
  return: FOF
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

