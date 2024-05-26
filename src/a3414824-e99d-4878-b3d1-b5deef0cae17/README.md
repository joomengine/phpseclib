```
██████╗  ██████╗ ██╗    ██╗███████╗██████╗
██╔══██╗██╔═══██╗██║    ██║██╔════╝██╔══██╗
██████╔╝██║   ██║██║ █╗ ██║█████╗  ██████╔╝
██╔═══╝ ██║   ██║██║███╗██║██╔══╝  ██╔══██╗
██║     ╚██████╔╝╚███╔███╔╝███████╗██║  ██║
╚═╝      ╚═════╝  ╚══╝╚══╝ ╚══════╝╚═╝  ╚═╝
```
# class Load (Details)
> namespace: **VastDevelopmentMethod\Joomla\Componentbuilder\Server**
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

