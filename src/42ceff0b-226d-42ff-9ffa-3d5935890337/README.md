```
██████╗  ██████╗ ██╗    ██╗███████╗██████╗
██╔══██╗██╔═══██╗██║    ██║██╔════╝██╔══██╗
██████╔╝██║   ██║██║ █╗ ██║█████╗  ██████╔╝
██╔═══╝ ██║   ██║██║███╗██║██╔══╝  ██╔══██╗
██║     ╚██████╔╝╚███╔███╔╝███████╗██║  ██║
╚═╝      ╚═════╝  ╚══╝╚══╝ ╚══════╝╚═╝  ╚═╝
```
# class Server (Details)
> namespace: **VDM\Joomla\Componentbuilder\Service**

```uml
@startuml
class Server  #Gold {
  + register(Container $container) : void
  + getServer(Container $container) : Client
  + getServerLoad(Container $container) : Load
  + getServerFtp(Container $container) : Ftp
  + getServerSftp(Container $container) : Sftp
}

note right of Server::register
  Registers the service provider with a DI container.

  since: 3.2.0
  return: void
end note

note right of Server::getServer
  Get the Server Client class

  since: 3.2.0
  return: Client
end note

note right of Server::getServerLoad
  Get the Server Load class

  since: 3.2.0
  return: Load
end note

note right of Server::getServerFtp
  Get the Server Ftp class

  since: 3.2.0
  return: Ftp
end note

note right of Server::getServerSftp
  Get the Server Sftp class

  since: 3.2.0
  return: Sftp
end note
 
@enduml
```

The Power feature in JCB allows you to write PHP classes and their implementations, making it easy to include them in your Joomla project. JCB handles linking, autoloading, namespacing, and folder structure creation for you.

By using the SPK (Super Power Key) in your custom code (replacing the class name in your code with the SPK), JCB will automatically pull the power from the repository into your project. This makes it available in your JCB instance, allowing you to edit it and include the class in your generated Joomla component.

JCB uses placeholders like [[[`NamespacePrefix`]]] and [[[`ComponentNamespace`]]] in namespacing to prevent collisions and improve reusability across different JCB systems. You can also set the **JCB powers path** globally or per component under the **Dynamic Integration** tab, providing flexibility and easy maintainability.

To add this specific Power to your project in JCB:

> simply use this SPK
```
Super---42ceff0b_226d_42ff_9ffa_3d5935890337---Power
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

