# Harbor Appliance

Create a Harbor instance on OpenStack and deploy with TLS support.

    virtualenv-3 venv
    source venv/bin/activate
    pip install -r requirements.txt
    ansible-galaxy install -r roles/requirements.yml -p roles
    ansible-playbook -i inventory install.yml

If you just wish to update projects and users:

    ansible-playbook -i inventory install.yml --start-at-task "Creating projects"
