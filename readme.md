
### belongsTo`/`Many to one

- [x] normal include filter
```json
  { "include": ["todoList"] }
```
- [x] where condition in related model
```json
{
  "include": [{
      "relation": "todoList",
      "scope": {
        "where": { "color": "black" }
      }
  }]
}
```

### hasMany`/`One to Many

- [x] normal include filter
```json
{
  "include": [{
    "relation": "todos"
  }]
}
```

- [x] where condition in related model
```json
{
  "include": [{
    "relation": "todos",
    "scope": { "where": { "isComplete": false } }
  }]
}
```

---
https://github.com/sourcefuse/loopback4-sequelize
