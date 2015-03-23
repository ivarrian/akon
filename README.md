# awsconnector

Simple utility to connect to EC2 instances based on the dashed naming scheme (example : foo-bar-1-dev )

# usage

	npm install
	./connector [--profile profileName] [--region awsRegion] arg1 [arg2] ... [argn]

# example

To connect to a single instance with the name tag : foo-bar-1-dev

	./connector foo bar 1 dev

To connect to multiple instances with name tag of pattern : foo-bar-*-dev

	./connector foo bar '*' dev

To connect to instances named foo-bar-* using profile work-stuff in region eu-west-1
	
	./connector --profile work-stuff --region eu-west-1 foo bar

# Tip

To use globally , simply add the path to your local repo in the PATH environment variable and use it like below: 

	connector arg1 [arg2] ... [argn]


# Bugs

Please report bugs at https://github.com/ivarrian/awsconnector/issues
