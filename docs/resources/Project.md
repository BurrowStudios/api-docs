# Project resource

## Project object

##### Project Structure

| Field   | Type                                                 | Description             |
|---------|------------------------------------------------------|-------------------------|
| id      | turtle                                               | The project's unique id |
| title   | string                                               | The project's title     |
| timings | [project timings](#Project-Timings-Structure) object | Timing information      |
| state   | one of [project state](#Project-State-Types)         | State of this project   |

##### Project Timings Structure

| Field   | Type       | Description                                                           |
|---------|------------|-----------------------------------------------------------------------|
| release | ?timestamp | The exact time the project will be / has been released (announced)    |
| apply   | ?timestamp | The exact time the project will be / has been opened for applications |
| start   | ?timestamp | The exact time the project will be / has been started                 |
| end     | ?timestamp | The exact time the project will be / has been ended or stopped        |

##### Project State Types

| Name        | Description                                                               |
|-------------|---------------------------------------------------------------------------|
| CONCEPT     | There has not been any planning yet, the project is merely an idea        |
| PLANNING    | The project is actively being planned                                     |
| APPLICATION | The project is done being planned and is currently accepting applications |
| RUNNING     | The project is currently running                                          |
| ENDED       | The project has ended as planned                                          |
| STOPPED     | The project has been stopped after it was already released                |
| CANCELED    | The project has been stopped before it was released                       |
