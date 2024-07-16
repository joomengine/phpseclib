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
  + iables $signature
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

The Power feature in JCB allows you to write PHP classes and their implementations, making it easy to include them in your Joomla project. JCB handles linking, autoloading, namespacing, and folder structure creation for you.

By using the SPK (Super Power Key) in your custom code (replacing the class name in your code with the SPK), JCB will automatically pull the power from the repository into your project. This makes it available in your JCB instance, allowing you to edit it and include the class in your generated Joomla component.

JCB uses placeholders like [[[`NamespacePrefix`]]] and [[[`ComponentNamespace`]]] in namespacing to prevent collisions and improve reusability across different JCB systems. You can also set the **JCB powers path** globally or per component under the **Dynamic Integration** tab, providing flexibility and easy maintainability.

To add this specific Power to your project in JCB:

> simply use this SPK
```
Super---11be6be3_ee3e_4771_8663_5545b76b73ab---Power
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

