<h1>Creating Infrastructure </h1>

## Commands
- "mkdir tf-code"
- "cp -a terraform-tests-1 tf-code"
- "cd tf-code/terraform-tests-1/"
- "curl -i http://127.0.0.1:8080/ -d "{\"description\":\"go skiing\",\"completed\":false}" -H 'Content-Type: application/spkane.todo-list.v1+json'"
- "terraform init"
- "terraform plan"
- "terraform apply"
- "curl http://127.0.0.1:8080/"
- "terraform output"
- "terraform state list"
- "terraform state show todo_todo.test1[2]"
- "curl http://127.0.0.1:8080/9"
- "terraform state pull"