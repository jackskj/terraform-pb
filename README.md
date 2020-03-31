# terraform-pb
Terrraform-pb allows the developer do manage their infrastructure programmatically with the language of their choice.
## Motivation
1) Flexibility: Many engineers prefer to manage their infrastructure with their favorite language, rather than relying on a data definition language.
This project allows just that. The developer can manage his/her infrastructure by instantiating a protocall buffer object which represents a terraform resource. 
2) Starting version 0.12, Terraform Core has adopted protocall buffers for communicating with each provider. More information [here](https://github.com/hashicorp/terraform/tree/master/docs/plugin-protocol). This adoption was taken to make provider development more [flexible and easier to manage](https://www.hashicorp.com/blog/announcing-the-terraform-plugin-sdk/). 
Doing the same between Terraform and end clients can be beneficial for the same reason.
## Notes
This is project is currently in development. What is available as of now are all resources and data types for each major providers in proto file definitions. 

I am currently workin on allowing the terraform end user to establish the connection with Terraform Core using the provider definitions. This will free the developer from using data definition language such as Hashicorp configuration language(HCL).

## Request for Comments

If you have thoughts, ideas, or comments about this project, please raise an issue.

## Providers
Below is the list of all available providers and their versions.
| Provider | Version |
|--|--|
|kubernetes |v1.11.1|
|azurerm |v2.3.0|
|aws |v2.55.0|
|google |v3.14.0|
|helm |v1.1.1|

