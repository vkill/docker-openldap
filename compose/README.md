### Run

```
ansible-playbook -i ansible_example/hosts -e "@ansible_example/var_prepare.yml" ansible_playbook_prepare.yml
```

```
docker-compose up
```

### Usage

```
xdg-open http://localhost:8080/

Login DN: cn=admin,dc=example,dc=org
Password: admin
```

```
ldapsearch -x -W -H ldap://localhost:389 -b "dc=example,dc=org" -D "cn=admin,dc=example,dc=org" "cn=admin"
```
