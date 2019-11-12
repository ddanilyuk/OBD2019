[PlantUML](http://plantuml.sourceforge.net/) is a component that allows to quickly write.
This is cheat sheet of PlantUML to use frequently.

# How to use PlantUML

## 1. Basic

### 1.1 Common

Notes and Comments.

| keyword        | usage               | image                                                        |
| -------------- | ------------------- | ------------------------------------------------------------ |
| `title``title` | Title               | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/title.png) |
| `note left :`  | Notes Left          | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/note_left.png) |
| `note right :` | Notes Right         | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/note_right.png) |
| `' `           | Single-line Comment |                                                              |
| `/' '/`        | Block Comment       |                                                              |

#### Code

```
title Title

( )
note left : Note

[  ]
note right : Note

' single-line comment

/'
  block comment
'/
```

#### Draw

 ![diagram1](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.github.com/ddanilyuk/OBD2019/master/documents/PlantUmlMarkdown/diagrams/1_1.puml)

### 1.2 Participant

Participant actors.

| keyword    | usage    | image                                                        |
| ---------- | -------- | ------------------------------------------------------------ |
| `actor`    | Actor    | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/element/actor.png) |
| `boundary` | Boundary | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/element/boundary.png) |
| `control`  | Control  | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/element/control.png) |
| `entity`   | Entity   | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/element/entity.png) |
| `database` | Database | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/package/database.png) |



#### Code

```
actor Actor
boundary Boundary
control Control
entity Entity
database Database

:Actor alias:
```

#### Draw

 ![diagram1](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.github.com/ddanilyuk/OBD2019/master/documents/PlantUmlMarkdown/diagrams/1_2.puml)


### 1.3 Arrow

Arrow direction.

| keyword    | usage | image                                                        |
| ---------- | ----- | ------------------------------------------------------------ |
| `-up->`    | Up    | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/up_line.png) |
| `-down->`  | Down  | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/down_line.png) |
| `-left->`  | Left  | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/left_line.png) |
| `-right->` | Right | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/right_line.png) |

#### Code

```
up -up-> right
-right-> down
-down-> left
-left-> up
```

#### Draw

 ![diagram1](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.github.com/ddanilyuk/OBD2019/master/documents/PlantUmlMarkdown/diagrams/1_3.puml)


## 2. UML

### 2.1 Use Case

Represent the required functions.

| keyword | usage           | image                                                        |
| ------- | --------------- | ------------------------------------------------------------ |
| `( )`   | Use Case        |                                                              |
| `->`    | Use             | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/use_line.png) |
| `.>`    | Extend, Include | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/ext_line.png) |

* [others](http://plantuml.sourceforge.net/usecase.html)

#### Code

```
actor Promoter
actor Entrant

Promoter --> (Create Event)
Promoter -> (Attend Event)

Entrant --> (Find Event)
(Attend Event) <- Entrant

(Attend Event) <.. (Create Member)  : <<include>>
```

#### Draw

 ![diagram1](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.github.com/ddanilyuk/OBD2019/master/documents/PlantUmlMarkdown/diagrams/2_1.puml)

### 2.2 Activity

Represent the state of the process.

| keyword  | usage    | image                                                        |
| -------- | -------- | ------------------------------------------------------------ |
| `" "`    | Activity | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/activity.png) |
| `(*) ->` | Initial  | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/initial_line.png) |
| `-> (*)` | Final    | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/final_line.png) |

* [others](http://plantuml.sourceforge.net/activity.html)

#### Code

```
(*) --> "Find Event"
"Find Event" -> "Attend Event"

if "Capacity?" then
  ->[ok] "Create Ticket"
else
  -->[full] if "Standby?" then
    ->[ok] "Standby Ticket"
  else
    -->[no] "Cancel Ticket"
    "Cancel Ticket" --> (*)
  endif
endif

"Create Ticket" --> ==show==
"Standby Ticket" --> ==show==
==show== --> "Show Ticket"
"Show Ticket" --> (*)
```

#### Draw

 ![diagram1](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.github.com/ddanilyuk/OBD2019/master/documents/PlantUmlMarkdown/diagrams/2_2.puml)

### 2.3 State

Represent the state of the objects.

| keyword  | usage   | image                                                        |
| -------- | ------- | ------------------------------------------------------------ |
| `[*] ->` | Initial | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/initial_line.png) |
| `-> [*]` | Final   | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/final_line.png) |

* [others](http://plantuml.sourceforge.net/state.html)

#### Code

```
[*] --> active

active -right-> inactive : disable
inactive -left-> active  : enable

inactive --> closed  : close
active --> closed  : close

closed --> [*]
```

#### Draw

 ![diagram1](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.github.com/ddanilyuk/OBD2019/master/documents/PlantUmlMarkdown/diagrams/2_3.puml)

### 2.4 Sequence

Represent the messages and  orders of the interacts.

| keyword | usage   | image                                                        |
| ------- | ------- | ------------------------------------------------------------ |
| `->`    | Message | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/message_line.png) |
| `<--`   | Return  | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/return_line.png) |

* [others](http://plantuml.sourceforge.net/sequence.html)

#### Code

```
actor Entrant

Entrant -> Ticket : Attend Event Request

activate Ticket
Ticket -> Member : Create Member Request

activate Member
Member -> Member : Create Member
Ticket <-- Member : Create Member Response
deactivate Member

Ticket -> Ticket : Create Ticket
Entrant <-- Ticket : Attend Event Response
deactivate Ticket
```

#### Draw

 ![diagram1](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.github.com/ddanilyuk/OBD2019/master/documents/PlantUmlMarkdown/diagrams/2_4.puml)

### 2.5 Object

Represent the logical view of the object.

| keyword  | usage       | image                                                        |
| -------- | ----------- | ------------------------------------------------------------ |
| `object` | Object      | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/object.png) |
| `<|-`    | Extension   | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/extension_line.png) |
| `*-`     | Composition | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/composition_line.png) |
| `o-`     | Agregation  | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/agregation_line.png) |

* [others](http://plantuml.sourceforge.net/objects.html)

#### Code

```
object User
object Group
object Member

object Event
object Ticket

User . Group
User o.. Member
Group o.. Member

Group o. Event
Event o.. Ticket
Member . Ticket
```

#### Draw

 ![diagram1](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.github.com/ddanilyuk/OBD2019/master/documents/PlantUmlMarkdown/diagrams/2_5.puml)

### 2.6 Class

Represent the logical view of the class.

| keyword | usage     | image                                                        |
| ------- | --------- | ------------------------------------------------------------ |
| `class` | Class     | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/class.png) |
| `+`     | Public    | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/public_visibility.png) |
| `-`     | Private   | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/private_visibility.png) |
| `#`     | Protected | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/protected_visibility.png) |
| `~`     | Package   | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/package_visibility.png) |

* [others](http://plantuml.sourceforge.net/class.html)

#### Code

```
class User {
  username
  password
  +sign_in()
}

class Group {
  name
}

class Member {
  roles
}

User .. Member
Group .. Member
```

#### Draw

 ![diagram1](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.github.com/ddanilyuk/OBD2019/master/documents/PlantUmlMarkdown/diagrams/2_6.puml)

### 2.7 Component

Represent the dependency of the components.

| keyword    | usage     | image                                                        |
| ---------- | --------- | ------------------------------------------------------------ |
| `[ ]`      | Component | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/parts/component.png) |
| `package`  | Package   | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/package/package.png) |
| `frame`    | Frame     | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/package/frame.png) |
| `folder`   | Folder    | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/package/folder.png) |
| `database` | Database  | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/package/database.png) |
| `node`     | Node      | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/package/node.png) |
| `cloud`    | Cloud     | ![parts_usecase](http://ogom.github.io/draw_uml/assets/img/diagrams/package/cloud.png) |

* [others](http://plantuml.sourceforge.net/component.html)

#### Code

```
cloud "Cloud" {
  package "Package" {
    [register]
    frame "frame" {
      [backup]
    }
  }
}

node "Node" {
  database "Database" {
    [store]
  }
  folder "Folder" {
    [File]
  }
}

[register] .. [store] : HTTP
[backup] .. [File] : FTP
```

#### Draw

 ![diagram1](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.github.com/ddanilyuk/OBD2019/master/documents/PlantUmlMarkdown/diagrams/2_7.puml)


### 2.8 Colors
We can add colors to Arrows, Icons, Sprites, Components, Packages, etc.
PlantUML support Hexadecimal colors or colors that are already defined.

Site Reference: http://plantuml.com/skinparam

#### Code

```
' =================
' == Declaration ==
' =================

[Component 1]

node "Node 1" {
    package "Package 1" #Orange {
        [Component 4]
        [Component 3]
    }
    [Component 2]
}



' ====================
' == Implementation ==
' ====================


node "Node 1" {
    [Component 2] .[#Green]-> [Component 4]
    [Component 3] <-left-> [Component 4]
    [Component 4] -- [Component 1]
}
```

#### Draw
 ![diagram1](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.github.com/ddanilyuk/OBD2019/master/documents/PlantUmlMarkdown/diagrams/2_8.puml)

### 2.9 Legends

Legend can contain only text, or some tables.
This example contain a table with some HTML inside and OpenIconic.

OpenIconic Reference: http://plantuml.com/openiconic

#### Code

```
legend
    |= Color |= Type |= Description |
    | <size:11><back:#Crimson>           </back></size>|    <&arrow-right> | Example 1 |
    | <size:11><back:#LightSeaGreen>           </back></size>|    <&arrow-right> | Example 2 |
    | <size:11><back:#DarkGreen>           </back></size>|    <&arrow-right> | Example 3 |
    | <size:11><back:#YellowGreen>           </back></size>|    <&box> | Example 4 |
    | <size:11><back:#Chocolate>           </back></size>|    <&box> | Example 5 |
endlegend
```

#### Draw
 ![diagram1](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.github.com/ddanilyuk/OBD2019/master/documents/PlantUmlMarkdown/diagrams/2_9.puml)


### 2.10 Constants
It's possible to declare constants that will help us for example to include files or other *.puml

PS: when you use it remove ${}, thats only there for the example

#### Code
```
!define ${VARIABLE NAME} ${VARIABLE VALUE}
```
