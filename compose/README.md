### Run

```
ansible-playbook -i ansible_example/hosts -e "@ansible_example/var_prepare.yml" ansible_playbook_prepare.yml
```

```
docker-compose up
```

### Usage

```
Open http://localhost:8080/
Login DN: cn=admin,dc=example,dc=org
Password: admin

Create Organisational Unit "Dev"

Create Posix Group "Dev"

Create User Account "heyongpeng" in "Dev" ou
```

```
sudo apt install ldap-utils
```

```
ldapsearch -x -W -H ldap://127.0.0.1:389 -b "ou=Dev,dc=example,dc=org" -D "cn=admin,dc=example,dc=org" "(cn=heyongpeng)"
# enter your ldap admin password
```
