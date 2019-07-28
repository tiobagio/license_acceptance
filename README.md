# License Acceptance Automated


See
https://github.com/chef-cft/effortless-infra-migration/blob/master/.kitchen.yml

Example of kitchen.yml which automatically accepts chef-license:

provisioner:
  name: chef_zero
  chef_client_path: /usr/bin/chef-client
  client_rb:
    chef_license: accept
    local_mode: true
  attributes:
    chef_license: accept
    effortless:
      origin: chef
      pkg: chef-client
      channel: unstable
