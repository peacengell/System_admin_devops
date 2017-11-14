# Aws cli with jq filterings 

## Need an account in aws
## Need to configure aws-secret key
## Need python aws


# My python aws  is install in a virtualenv.

 - aws ec2 describe-instances 

    Running the above command will dump everythings in the EC2 instance as a json file.
    We need to save it into a file so we work on the file instead calling the same json each time, as we are learning how to filter using jq.
    The commande below will save the outout to the file, as now on we will work with this file.
    
 - aws ec2 describe-instances >describe_instance.json

 - cat describe_instance.json | jq [options]



