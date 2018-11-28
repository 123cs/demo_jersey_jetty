# JettyWithJerseyHomework

This repo is an example of a RESTful API using Jetty & Jersey.

# demo.Note
  - id
  - content
  - created_by
  - created_date
  - lastupdated_by
  - lastupdated_date

# API Instruction
- Create a new demo.Note:

  POST method to /note
  
  Header 
  
    Content-Type: application/type
    
  Body
  
      {
        "content" : "demo.Note content",
        "created_by" : "username"
      }

- Get demo.Note by Id

  GET method to /note/:id

- Get all demo.Note

  GET method to /note

- Search notes

  GET method to /note/search
  
  Query params:
  
    + created_by
    + from (long value only
    + content

- Edit demo.Note by Id

  PUT method to /note/:id
  
      {
        "content" : "demo.Note content",
        "lastupdated_by" : "username"
      }

- Delete demo.Note By Id

  DELETE method to /note/:id
