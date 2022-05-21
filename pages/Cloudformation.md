- Iac service
- YAML or JSON
- Cloudformation handles the order of deployment and know the dependancies
- Components of Cloudformation
  collapsed:: true
	- Stack
		- A set of resource that you can provision, update or delete
	- Templates
		- JSON or YAML file where you describes the resources that to be created
	- Stack set
		- Allows you to update delete or create your stacks across a number of AWS accounts in different regions with a single template
		- You select the Template and which regions
		- #+BEGIN_IMPORTANT
		  In order to delete the stack set you need to ensure to delete all the stack instances in it
		  #+END_IMPORTANT
	- Stack instances
		- Each individual stacks created under stackset on multi regions are called as stack instances
	-