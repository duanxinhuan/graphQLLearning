# graphQLLearning
A learning repo for graphql, LOL :) feel free to copy my notes, glhf
#Schema

## Simple Schema

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
