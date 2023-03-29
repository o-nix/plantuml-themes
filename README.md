# PlantUML Themes

https://plantuml.com/theme

```puml
!theme drawio from https://raw.githubusercontent.com/o-nix/plantuml-themes/main/

actor Actor
participant Component
queue Queue
participant Worker <<decides what to do>>
collections Nodes

Actor -> Component: Message

group Important
  Component -> Queue: Publish message
  note right of Queue: Message\nis meaningful
  Queue -> Worker: Pick up message
  Worker -> Nodes: Do something
end
```

![image](https://user-images.githubusercontent.com/647149/228601021-be74241d-acec-4602-a09a-21bf91b83461.png)

