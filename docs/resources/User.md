# User resource

## User object

##### User Structure

| Field     | Type                | Description                            |
|-----------|---------------------|----------------------------------------|
| id        | turtle              | The user's unique id                   |
| name      | string              | The user's display name                |
| discord   | array of snowflakes | Discord accounts linked to this user   |
| minecraft | array of UUIDs      | Minecraft accounts linked to this user |
