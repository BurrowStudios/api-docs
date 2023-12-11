# Ticket resource

## Ticket object

##### Ticket Structure

| Field | Type                                       | Description                                        |
|-------|--------------------------------------------|----------------------------------------------------|
| id    | turtle                                     | The ticket's unique id                             |
| title | ?string                                    | Title of this ticket (if set by user or moderator) |
| state | one of [ticket state](#Ticket-State-Types) | State of this ticket                               |
| tags  | array of strings                           | Additional tags added by user or moderator         |
| users | array of [user](User.md) ids               | Users that are involved in this ticket             |

##### Ticket State Types

| Name     | Description                                           |
|----------|-------------------------------------------------------|
| OPEN     | Ticket is not yet resolved and has not been abandoned |
| RESOLVED | Ticket and underlying issue are resolved              |
| FROZEN   | Ticket cannot be resolved at the time                 |
| CLOSED   | Ticket has been abandoned                             |
| DRAFT    | Ticket is not yet open                                |
