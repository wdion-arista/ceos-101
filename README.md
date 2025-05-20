# cEOS-lab 101

This is a repository to help getting started with cEOS-lab in Containerlab.

- Run containerlab in your local machine pointing to the YAML file URL.
  
      clab deploy -t https://github.com/diogo-arista/ceos-101/blob/main/topology.yaml
      18:53:38 INFO Containerlab started version=0.68.0
      18:53:38 INFO Parsing & checking topology file=topology.yaml
      18:53:38 INFO Creating docker network name=clab IPv4 subnet=172.20.20.0/24 IPv6 subnet=3fff:172:20:20::/64 MTU=1500
      18:53:38 INFO Creating lab directory path=/home/diogo/ceos-101/ceos-101/clab-sample
      18:53:38 INFO Creating container name=ceos2
      18:53:38 INFO Creating container name=ceos1
      18:53:39 INFO Running postdeploy actions for Arista cEOS 'ceos1' node
      18:53:39 INFO Created link: ceos1:eth1 ▪┄┄▪ ceos2:eth1
      18:53:39 INFO Running postdeploy actions for Arista cEOS 'ceos2' node
      18:53:52 INFO Adding host entries path=/etc/hosts
      18:53:52 INFO Adding SSH config for nodes path=/etc/ssh/ssh_config.d/clab-sample.conf
      ╭───────┬──────────────┬─────────┬───────────────────╮
      │  Name │  Kind/Image  │  State  │   IPv4/6 Address  │
      ├───────┼──────────────┼─────────┼───────────────────┤
      │ ceos1 │ ceos         │ running │ 172.20.20.3       │
      │       │ ceos:4.33.2F │         │ 3fff:172:20:20::3 │
      ├───────┼──────────────┼─────────┼───────────────────┤
      │ ceos2 │ ceos         │ running │ 172.20.20.2       │
      │       │ ceos:4.33.2F │         │ 3fff:172:20:20::2 │  
      ╰───────┴──────────────┴─────────┴───────────────────╯
  
- You may clone this repository in your local machine.
- Reopen the repository in a container locally.
- Open the repository in a container on Github Codespaces.
  
Follow the Arista Community Central article below for more information:
"Link"
