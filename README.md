# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
  ExampleParent <|-- ExampleChild
  class ExampleParent{
        - name: string
        - email: string
        - password: string
        + login(user: string, pass: string) boolean
        + get_email() string
  }
  class ExampleChild{
        - badges vector~string~
        + add_badge(title: string)
        + get_badges() vector~string~
  }
```
## Data model 2

```mermaid
classDiagram 
      TypeCoach <|-- TypeStudent   
      class TypeCoach{
            -id: string
            +create_lesson()string
      }
      class TypeStudent{
            -name: string
            -email: string
            -level: integer
            -problem_keys: string
            + get_email() string
      }
      
