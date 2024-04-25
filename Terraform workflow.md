<h1>Terraform Workflow </h1>

## Initialization
- Typically the first thing you want to do is "terraform init"
- This takes a look at the code in the current directory and makes sure you have all dependacies that you need available
- Initializes the backend to store the stae file ypically on the cloud but can be local
- Grabs plugins required
- Once initialization is done a lock file is created to record what provider versions were installed

## Plan/Apply
- A terraform plan is a dry run which makes a call to all of the API's 
- Provides a list of all the changes it will make 
- can choose to apply or not
- To apply these changes you can use "terraform apply"
- This runs plan again and confirms you want to apply but you can set automatic approvals
- Then will display an outputs on what was added/changed/destroyed

## Output
- "Terraform output" will print out all outputs that are defined
- This can be useful for other pipelines or users to use

## State list
- "Terraform state list" will show all objects defined in the state file
- For a specific object you can use "terraform state show objectname"

## Destroy
- "Terraform destroy" tears down all infrastructre defined and spun up
- Confirms that the infrastructure exists and asks for confirmation for delete
- Deletes in reverse dependacy order to delete as cleanly as possible





