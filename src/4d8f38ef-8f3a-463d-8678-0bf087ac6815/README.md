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

The Power feature in JCB allows you to write PHP classes and their implementations, making it easy to include them in your Joomla project. JCB handles linking, autoloading, namespacing, and folder structure creation for you.

By using the SPK (Super Power Key) in your custom code (replacing the class name in your code with the SPK), JCB will automatically pull the power from the repository into your project. This makes it available in your JCB instance, allowing you to edit it and include the class in your generated Joomla component.

JCB uses placeholders like [[[`NamespacePrefix`]]] and [[[`ComponentNamespace`]]] in namespacing to prevent collisions and improve reusability across different JCB systems. You can also set the **JCB powers path** globally or per component under the **Dynamic Integration** tab, providing flexibility and easy maintainability.

To add this specific Power to your project in JCB:

> simply use this SPK
```
Super---4d8f38ef_8f3a_463d_8678_0bf087ac6815---Power
```
> remember to replace the `---` with `___` to activate this Power in your code

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

