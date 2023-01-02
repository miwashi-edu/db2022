# db2022

## Beskrivning

I kursen DB2022 på IT-Högskolan skulle vi redovisa på färdigheter i SQL, Normalisering samt Java mot en relationsdatabas. Detta är min redovisning från denna kurs.

[Mermaid](https://mermaid-js.github.io/mermaid/#/entityRelationshipDiagram)


## Entity Relationship Diagram

```mermaid
erDiagram
    Student ||--|{ StudentSchool : enrolls
    School ||--|{ StudentSchool : accepts
    
    StudentSchool {
        int StudentId
        int SchoolId
    }
    
    Student {
        int StudentId
        string FirstName
        string LastName
    }
    
    School {
        int SchoolId
        string Name
        string City
    }
    
```

## Cardinality

![Cardinality](cardinality-1.png)
