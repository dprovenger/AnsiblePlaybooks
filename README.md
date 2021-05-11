# AnsiblePlaybooks

# Creating installer document
aws ssm create-document \
--name "install-docker" \
--content file://install-docker.yml \
--document-type "Command" \
--document-format YAML \
--region eu-west-1


# Creating automation document
aws ssm create-document \
--name "install-docker" \
--content file://automate-docker.yml \
--content-type "Automation" \
--document-format YAML \ 
--region eu-west-1