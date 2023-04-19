# Ansible Solution

Possible solution for ansible part
Disclaimer: Tested with ansible 2.14.4

## Changes to be done for let it work

- Put jboss-eap in ansible/roles/jboss.install/files
- Change jboss version when needed in ansible/roles/jboss.install/defaults/main.yml
- Change networkadapter settings:
  ansible/roles/webservers/templates/site_index.j2:  \<h2\>Running on address: \{\{ ansible_enp0s1\.ipv4\.address \}\}\<\/h2\>
  ansible/roles/webservers/templates/index.j2:\<h2\>Running on address: \{\{ ansible_enp0s1\.ipv4\.address \}\}\<\/h2\>
  ansible/roles/haproxy.install/templates/haproxycfg.j2:    server \{\{ hostvars\[host\]\['ansible_hostname'\] \}\} \{\{ hostvars\[host\]\['ansible_enp0s1'\]\['ipv4'\]\['address'\] \}\}:\{\{ app_port \}\} check
  ansible/templates/index.j2:\<h2\>Running on address: \{\{ ansible_enp0s8\.ipv4\.address \}\}\<\/h2\>
