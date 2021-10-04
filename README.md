
# Overview

Only changes I made are in [cdk_hello/cdk_hello_stack.py](cdk_hello/cdk_hello_stack.py) to
- create s3 bucket
- create entire ecs stack with VPC, ALB etc(!) in a couple lines

Note  I also removed cdk.out from .gitignore since I was thinking about keeping resulting CFN under version control for use via Rio

# Requirements & Running

- python & pip
- brew install aws-cdk
- virtualenv . ./.venv/bin/activate
- pip install -r requirements.txt
- cdk synth/deploy/diff/destroy

# More doco
- https://docs.aws.amazon.com/cdk/latest/guide/getting_started.html
- https://pypi.org/project/aws-cdk.aws-ecs-patterns/
