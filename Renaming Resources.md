<h1>Renaming resources</h1>

## Move block method
- create block 
  moved{
  from = todo_todo.imported
  to   = todo_todo.primary
  }
- "terraform plan"
- "terraform apply"
- **advantage**
    - allows CI/CD systems to do these changes removing human risk factor
- **Disadvantage**
    - can lead to clutter in the terraform file

## State move command
- "terraform state mv todo_todo.imported todo_todo.primary
- easy to use but requires Human to run command

