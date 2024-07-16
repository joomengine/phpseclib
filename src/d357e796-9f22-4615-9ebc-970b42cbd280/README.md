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

The Power feature in JCB allows you to write PHP classes and their implementations, making it easy to include them in your Joomla project. JCB handles linking, autoloading, namespacing, and folder structure creation for you.

By using the SPK (Super Power Key) in your custom code (replacing the class name in your code with the SPK), JCB will automatically pull the power from the repository into your project. This makes it available in your JCB instance, allowing you to edit it and include the class in your generated Joomla component.

JCB uses placeholders like [[[`NamespacePrefix`]]] and [[[`ComponentNamespace`]]] in namespacing to prevent collisions and improve reusability across different JCB systems. You can also set the **JCB powers path** globally or per component under the **Dynamic Integration** tab, providing flexibility and easy maintainability.

To add this specific Power to your project in JCB:

> simply use this SPK
```
Super---d357e796_9f22_4615_9ebc_970b42cbd280---Power
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

