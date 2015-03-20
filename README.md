# awsconnector

Simple utility to connect to EC2 instances based on the dashed naming scheme (example : foo-bar-1-dev )

# usage

	npm install
	./connector arg1 [arg2] ... [argn]

# example

To connect to a single instance with the name tag : foo-bar-1-dev

	./connector foo bar 1 dev

To connect to multiple instances with name tag of pattern : foo-bar-*-dev

	./connector foo bar '*' dev

# Tip

To use globally , simply add the path to your local repo in the PATH environment variable and use it like below: 

	connector arg1 [arg2] ... [argn]


# Bugs

Please report bugs at https://github.com/ivarrian/awsconnector/issues
