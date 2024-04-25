<h1>Using Terrafrorm modules</h1>

## Terrafrorm modules
- A way to organise terraform code so you are not repeating yourself throughout the codebase
- Allows you to standardize how teams spin up infrastructure
- Typical difference of a module and standard code is that it needs more variables to be available to wider teams.
- Needs to be flexible to for the needs of many teams but also follow best practices
- In module your variables can be thought of as inputs especially if they dont have defaults and your outputs as your returns
 
## Commands
- cp -a __modules/ tf-code/
- apply code changes
- terraform init
- terraform plan
- terraform apply
- curl http://127.0.0.1:8080/23
- terraform destroy

## Code to add
- **main.tf**

```

Module "series-data" {
    source        = "../__modules/todo-test-data"
    number        = 5
    purpose       = "testing"
    team_name     = "oreilly"
    descriptions  = ["my first completed todo", "my second completed todo", 
                     "my third completed todo", "my fourth completed todo",
                     "my fifth completed todo"]
}
- **outputs.tf**

```

- **outputs.tf**

```

output "first_series_ids" {
  value = module.series-data.frist_series_ids
}
output "second_series_ids" {
  value = module.series-data.second_series_ids
}

```
