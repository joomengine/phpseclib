```
██████╗  ██████╗ ██╗    ██╗███████╗██████╗
██╔══██╗██╔═══██╗██║    ██║██╔════╝██╔══██╗
██████╔╝██║   ██║██║ █╗ ██║█████╗  ██████╔╝
██╔═══╝ ██║   ██║██║███╗██║██╔══╝  ██╔══██╗
██║     ╚██████╔╝╚███╔███╔╝███████╗██║  ██║
╚═╝      ╚═════╝  ╚══╝╚══╝ ╚══════╝╚═╝  ╚═╝
```
# class Load (Details)
> namespace: **VDM\Joomla\Componentbuilder\Server**

```uml
@startuml
class Load  #Gold {
  # Database $db
  # Model $model
  + __construct(?Database $db = null, ?Model $model = null)
  + value(int $id, string $field) : mixed|null
  + item(int $id, array $fields) : ?object
  # setDatabaseFields(array $fields, string $key = 'a') : array
}

note right of Load::__construct
  Constructor

  since: 3.2.0
end note

note right of Load::value
  Get a value from a given server
Example: $this->value(23, 'protocol');

  since: 3.2.0
  return: mixed|null
end note

note right of Load::item
  Get values from a given server
Example: $this->item(23, ['name', 'of', 'fields']);

  since: 3.2.0
  return: ?object
end note

note right of Load::setDatabaseFields
  Set Fields ready to use in database call

  since: 3.2.0
  return: array
end note
 
@enduml
```

The Power feature in JCB allows you to write PHP classes and their implementations, making it easy to include them in your Joomla project. JCB handles linking, autoloading, namespacing, and folder structure creation for you.

By using the SPK (Super Power Key) in your custom code (replacing the class name in your code with the SPK), JCB will automatically pull the power from the repository into your project. This makes it available in your JCB instance, allowing you to edit it and include the class in your generated Joomla component.

JCB uses placeholders like [[[`NamespacePrefix`]]] and [[[`ComponentNamespace`]]] in namespacing to prevent collisions and improve reusability across different JCB systems. You can also set the **JCB powers path** globally or per component under the **Dynamic Integration** tab, providing flexibility and easy maintainability.

To add this specific Power to your project in JCB:

> simply use this SPK
```
Super---a3414824_e99d_4878_b3d1_b5deef0cae17---Power
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

