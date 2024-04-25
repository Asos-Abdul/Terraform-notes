<h1>HCL components </h1>

## Main.tf 
 - HCL is made up of blocks with typically key value pairs
 - Provides high level configuration such as specifying required versions
 - Define provider sources and versions
 - Can define our backend and give details required to connect to our remote cloud storage or local storage
 - You should always try to have a remote backend
 - use variables to provide API keys to avoid hardcoding secrets

 ## variables.tf
 - Blocks that define variables
 - **Variable types**
    - String
    - number
    - list
    - bool
    - set
    - map
    - null
- Descriptions to help people understand what the variables are for
- You can define defaults to differentiate between required variables and unrequired

## Backend.tf
- A resource block is the most important compnent of terraform
- resource "resource type" "resource name" is the layout
- resources are thing you want to create and manage with terraform
- contains everything we need to pass to have it created through the API

## Data.tf
- Data sources are read only API objects
- Important when you want information that you dont control or manage

## Output.tf
- outputs are stored in output.tf
- output blocks point to a value that was created when creating an API object

## State file
- "terraform state pull" will pull down the file from wherever it is stored
- displays all resources, data and outpus





