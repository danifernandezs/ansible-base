# Ansible Base

Install dependencies with:

```
$ ansible-galaxy role install \
  --role-file requirements.yml \
  --force
```

```
$ ansible-galaxy collection install \
  --requirements-file requirements.yml \
  --force
```

Insert your credentials:

```
$ cp inventory/group_vars/all/credentials.yml.sample inventory/group_vars/all/credentials.yml
$ vi inventory/group_vars/all/credentials.yml
```

Run a playbook:

```
$ ansible-playbook -i inventory/localhost.yml <playbook>
```

# Local execution environment requirements

RPM package
```bash
python3-passlib
```

Via pip
```bash
openshift
pyyaml
kubernetes
```
