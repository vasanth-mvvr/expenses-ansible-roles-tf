# ** Ansible Configuration **

# There are various ways of setting ansible configuration

# 1) First one is environment variables
# ANSIBLE_CONFIG for this we can set using export 
```
export ANSIBLE_CONFIG=/tmp/ansible.cfg
```
# Note: In the above we have copied the ansible version and placed in the variable 
# 2) To unset
```
unset ANSIBLE_CONFIG        
```
# Note: It comes to the default that is /etc/ansible/ansible.cfg

# To set in current directory
```
ansible.cfg
```
# To set in root directory
```
~/.ansible.cfg 
```
# Note: ~/ is home directory and .ansible.cfg is hidden file in home directory

# ** Ansible vault is used for securing passwords **

# creation of vault
```
ansible-vault create <filename.yaml>
```

# Viewing of vault
```
ansible-vault view <filename.yaml>
```

# Editing of vault
```
ansible-vault edit <filename.yaml>
```
# ** IAM - Identity access and management**

# create a user collect the access key credentials copy it and use aws configure command
```
aws configure
```
# For checking
```
aws s3 ls
```
