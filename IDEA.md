# Geronimo - Simple task/bug tracker

## User roles:
- admin: default user, can do everything, cannot be deleted
- leader: admin for the project, assigned by admin, can do everything within the assigned project, can assign other users for the project
- doer: can do everything with the assigned tasks (move, comment, attach files), can watch for the assigned project (comment other tasks)
- spectator (can only watch for the assigned project)

## Features:
- many boards with custom stages
- two types of entities: task and bug
- drag-and-drop for entities
- entity can contain sub-entities, but only the first level of sub-entities will be shown
- entities can be moved to another stage by drag-and-drop, sub-entities - only by changing of their status
- sub-entities have the same stages as the project
- ability to add comments and files to the entity
- multiple assignee for an entity
- entities can be moved left or right only on one step at the time
- all the movings of entities must be logged (task, user, status, timestamp)
- entity must have next fields, assigned by the leader:
    - severity
    - urgency
    - complexity
    - deadline 
- only empty stages can be deleted

## Technologies to use:
- django
- react
- ant design
- postgresql
- docker compose
