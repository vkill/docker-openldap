### Usage

```
cp ansible_hosts.example ansible_hosts
cp ansible_var_prepare.yml.example ansible_var_prepare.yml
```

```
bash ansible_playbook_prepare.sh -e "@ansible_var_prepare.yml" -i ansible_hosts
```

```
cd /data/data_openldap/compose_project
bash docker-compose.sh up
```

```
xdg-open http://localhost:8080/

Login DN: cn=admin,dc=example,dc=org
Password: admin
```

```
ldapsearch -x -W -H ldap://localhost:389 -b "dc=example,dc=org" -D "cn=admin,dc=example,dc=org" "cn=admin"
```
