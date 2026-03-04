# tippitytappity-design

tippitytappity is a program to practice typing



## Data model 2 Revision


It keeps a history of each typing test the user attempts including the results (both accuracy and speed)
Supports multiple users, with history for each user to monitor their progress over time

```mermaid 
classDiagram
      User -->TypeChecker
      class User{
            -name: string
            -email: string
            -level: integer
            +typeHIstory: string
            +typeTime: integer
            +typeLevel: integer
      }
      class TypeChecker{
            -id_checker : string
            -solution: string
            +get_Accuracy(typeHistory, solution  )
            +get_problemKeys(typeHistory, solution)
            +get_typingSpeed(typeTime, typeHistory)


      }
      TypeChecker -->ProgressChecker
      class ProgressChecker{
            -id : integer
            +getProgress()

      }


```

