# graphQLLearning
A learning repo for graphql, LOL :) feel free to copy my notes, glhf

## 1. Concepets
- SDL:schema definition language

## 2. Schemas

### 2.1 Schema Defination

```python
#this is actually not python code, just make it python for convinience!
type person{
  name: String!,
  age: int,
  posts:[post]!
}

type post{
  tile: String!,
  author: person,
}
```

### 2.2 Schema for Query

```python
#this is actually not python code, just make it python for convinience!
{
    allPersons{
        name,
    }
}

# In graphql, create delete updating are called mutations
type mutation{
    createPerson(name: "Bob", age: 36){
        name person
    }
    updatePerson()
    deletePerson()
}

#update like stream

type subscription{
    newPerson{
        name,
        age
    }
}

#query

type Query{
    allPersons(last:int) : [Person]!
}
```

## Architectural Use Cases
