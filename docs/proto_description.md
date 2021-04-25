## Commands

|   Code   | Command        | Fields                    | Data                                     |
| :------: | -------------- | ------------------------- | ---------------------------------------- |
| `0x0000` | sign in        |                           | username                                 |
| `0x0100` | get lists      | user_id                   |                                          |
| `0x0101` | create list    | user_id                   | name                                     |
| `0x0102` | delete list    | user_id, list_id          |
| `0x0103` | edit list data | user_id, list_id          | name                                     |
| `0x0110` | get tasks      | user_id, list_id          |
| `0x0111` | create task    | user_id, list_id          | title, created_at, description, deadline |
| `0x0112` | delete task    | user_id, list_id, task_id |
| `0x0113` | edit task      | user_id, list_id, task_id | title, description, deadline             |

## Responses

|   Code   | Description    |
| :------: | -------------- |
| `0x0000` | success        |
| `0x0001` | already exists |
| `0x0002` | not found      |
