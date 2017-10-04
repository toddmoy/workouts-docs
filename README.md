Workouts Docs
=============

API
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
}
```
