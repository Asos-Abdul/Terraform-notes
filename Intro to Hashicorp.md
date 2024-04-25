<h1>Intro to hashiorp </h1>

## What is Terraform
- Comes from the verb of altering a planet for the purpose of sustaining life
- Compare the potential resources that cloud and software provide to companies as the resources available on any planet
- We convert these resouces into a form that is useful and group them in a way that they provide benefits
- In Computer infra terms it is a tool that can define and manage the lifecycke of any API based infra stack
- Utilizes the the API of onlince services(e.g.AWS, Github, K8, etc) to control the life cycle of each component defined
- Also possible to extend so it can run with custom API's 
- Once Initial code is created teams across a organisation can easily spin up and maintain complex infrastructure

## Modules
- Modules make it possible to create a reusable package of terraform code that can simplify the work required from end users
- Makes it possible to ensure that infrastructure standards are maintained acrross an organisation
- Can be used to ensure labels for components are applied or files in the cloud storage are encrypted at rest

## HCL
- Terraform defines infrastuculr usin hashiorp configuration language(HCL) 
- A DSL(domain specific language) similar to JSON or YAML
- Designed to solve problems  inherent in both JSON and YAML while mainitain compatability
- supports comments unlike JSON and more forgiving with indentation unlike YAML
- Makes it the ideal way to decribe infrastructure

## Terminology
- **State file**
    -  A JSON file that contains all the data terraform requires to manage a lifecyle of an infratructure stack
- **Backend**
    - The system used to store the state file
- **Providers**
    - Plugins that enable terraform to work with specifc API'services
- **Variables**
    - Passed into codebase to modify how it behaves
- **Resources**
    - Each resource represents a single API object to be managed
- **Data sources**
    - Read-only form of a resource that is defined by a Providers
    - Used to compare required values
- **Outputs**
    - Data that can be passed out of module for consumption by users or other modules