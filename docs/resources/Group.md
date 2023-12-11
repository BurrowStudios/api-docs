# Group resource

## Group object

##### Group Structure

| Field    | Type                         | Description                           |
|----------|------------------------------|---------------------------------------|
| id       | turtle                       | The group's unique id                 |
| name     | string                       | The group's display name              |
| size     | integer                      | Amount of members in this group       |
| members  | array of [user](User.md) ids | Users that are a member of this group |
| position | integer                      | Position of this group in group lists |