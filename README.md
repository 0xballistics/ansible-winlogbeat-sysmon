# ansible-winlogbeat-sysmon
Ansible role for installing winlogbeat and sysmon

### example playbook
```yaml
- hosts: win
  tasks:
    - import_role:
        name: ansible-winlogbeat
      vars:
        elasticsearch_host: "192.168.56.1:9200"
        kibana_host: "192.168.56.1:5601"
        # force_install: true
```

### configurations
WinLogBeat: [Malware Archeology WinLogBeat configuration file](https://www.malwarearchaeology.com/s/winlogbeat-8e78.yml).
Sysmon: [SwiftOnSecurity sysmon config](https://github.com/SwiftOnSecurity/sysmon-config).
