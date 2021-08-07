# Azure testing with ansible

Basic playbook, mostly from Ansible documentation

```
$ virtualenv env-azure
$ . env-azure/bin/activate
$ pip3 install -r requirements.txt
$ pip3 install -r https://raw.githubusercontent.com/ansible-collections/azure/dev/requirements-azure.txt
$ ansible-galaxy collection install azure.azcollection
$ ansible-playbook -v azurelab-test.yml
```

If using the SQL import, need freetds library
```
$ brew install freetds
```

## Other playbooks

* azure-database: test SQL server with some security settings

* azure-sentinel-simple: basic log analytics and sentinel
* azure-sentinel-az2go with https://github.com/OTRF/Azure-Sentinel2Go

* azure-jumphost: Linux Jumphost with some system hardening and docker

## References

* [installing ansible[azure] in same pip command as ansible doesn't work #67255](https://github.com/ansible/ansible/issues/67255#issuecomment-621408450)

## License

BSD 2-clause
