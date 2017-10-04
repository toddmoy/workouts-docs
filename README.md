Workouts Docs
=============

1 ROUTES
------

```
/

/workouts
/workouts/:id
/workouts/:id/edit
/workouts/new
/workouts/delete

/exercises
/exercises/:id
/exercises/:id/edit
/exercises/new
/exercises/delete

/settings
```


2 API
---

**Exercises**

An exercise is a single activity that an athlete will perform. Often they are repeated in sets. 
 
```json
// Example

{
  "id": 1,
  "title": "7-second Hangs",
  "description": "Hang for 7 seconds, then rest for 3. Make sure your shoulders are engaged.",
  "type": "Hangboard",
  "equipment": "Hangboard",
  "timerSettings": [
    {"countdown": 10},
    {"active": 7},
    {"rest": 3},
    {"restBetweenSets": 500},
  ],
  "targets": [
    {"body": "fingers"},
    {"performance": "strength"}
  ]
}
```

**Routine**

A routine is a collection of `Exercises` that are performed sequentially. 

```json
// Example
{
 "id": 1,
 "title": "Hangboard Workout #1",
 "description": "",
 "agenda": [
  { 
   "title": "7-second Hangs",
   "difficulty": "Jug",
   "complete": false
  },{
    "title": "7-second Hangs",
    "difficulty": "Inside VDR",
    "complete": false
  }
 ]
}
```

**User**

```json
{
  "id": 1,
  "firstName": "Todd",
  "lastName": "Moy",
  "avatar": "//placehold.it/500x500/"
}
```
