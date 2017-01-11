# Ansible API
This is a really simple ansible API written in Flask

If you are looking for a fully fledged API, take a look at Ansible Tower

This Flask app lets you look at your roles via the api, and lets you run playbooks via the API

An example role is included to run a test to ensure the system is functioning

    curl --request POST \
      --url http://127.0.0.1:8080/api/run/ \
      --data 'role=test' \
      --data 'play=hello.yml'
      --data 'host=localhost'
      

You can follow this test example to run your Ansible Role. 

The role parameter relates to the directory your role is in
The play parameter is the Ansible playbook you want to run
The host parameter is the host you want to run the play against

This is honestly just some code I threw together to see if I could write an API that actually does something, as it turns out
I can 

Thanks for checking it out

~D
