# AKON (formerly awsconnector)

AKON as in **A**WS **KON**ector

Simple utility to connect to EC2 instances based on the dashed naming scheme (example : foo-bar-1-dev )

# usage

	npm install
	./akon [--profile profileName] [--region awsRegion] arg1 [arg2] ... [argn]

# example

To connect to a single instance with the name tag : foo-bar-1-dev

	./akon foo bar 1 dev

To connect to multiple instances with name tag of pattern : foo-bar-*-dev

	./akon foo bar '*' dev

To connect to instances named foo-bar-* using profile work-stuff in region eu-west-1
	
	./akon --profile work-stuff --region eu-west-1 foo bar

# Tip

To use globally , simply add the path to your local repo in the PATH environment variable and use it like below: 

	akon arg1 [arg2] ... [argn]


# Bugs

Please report bugs at https://github.com/ivarrian/awsconnector/issues