# cEOS-lab 101

This is a repository to help getting started with cEOS-lab in Containerlab.

- Run containerlab in your local machine pointing to the YAML file URL:
```
clab deploy -t https://github.com/diogo-arista/ceos-101/blob/main/topology.yaml
```
Example:
```
diogo@clab-debian:~/ceos-101$ clab deploy -t https://github.com/diogo-arista/ceos-101/blob/main/topology.yaml
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
```

- You may clone this repository in your local machine:
```
git clone https://github.com/diogo-arista/ceos-101.git
```
Example:
```
diogo@clab-debian:~$ git clone https://github.com/diogo-arista/ceos-101.git
Cloning into 'ceos-101'...
remote: Enumerating objects: 54, done.
remote: Counting objects: 100% (54/54), done.
remote: Compressing objects: 100% (45/45), done.
remote: Total 54 (delta 10), reused 25 (delta 3), pack-reused 0 (from 0)
Receiving objects: 100% (54/54), 11.73 KiB | 3.91 MiB/s, done.
Resolving deltas: 100% (10/10), done.
diogo@clab-debian:~$ cd ceos-101/
diogo@clab-debian:~/ceos-101$ clab deploy -t topology.yaml 
19:08:15 INFO Containerlab started version=0.68.0
19:08:15 INFO Parsing & checking topology file=topology.yaml
19:08:15 INFO Creating docker network name=clab IPv4 subnet=172.20.20.0/24 IPv6 subnet=3fff:172:20:20::/64 MTU=1500
19:08:15 INFO Creating lab directory path=/home/diogo/ceos-101/clab-sample
19:08:15 INFO Creating container name=ceos2
19:08:15 INFO Creating container name=ceos1
19:08:15 INFO Running postdeploy actions for Arista cEOS 'ceos1' node
19:08:15 INFO Created link: ceos1:eth1 ▪┄┄▪ ceos2:eth1
19:08:15 INFO Running postdeploy actions for Arista cEOS 'ceos2' node
19:08:28 INFO Adding host entries path=/etc/hosts
19:08:28 INFO Adding SSH config for nodes path=/etc/ssh/ssh_config.d/clab-sample.conf
╭───────┬──────────────┬─────────┬───────────────────╮
│  Name │  Kind/Image  │  State  │   IPv4/6 Address  │
├───────┼──────────────┼─────────┼───────────────────┤
│ ceos1 │ ceos         │ running │ 172.20.20.3       │
│       │ ceos:4.33.2F │         │ 3fff:172:20:20::3 │
├───────┼──────────────┼─────────┼───────────────────┤
│ ceos2 │ ceos         │ running │ 172.20.20.2       │
│       │ ceos:4.33.2F │         │ 3fff:172:20:20::2 │
╰───────┴──────────────┴─────────┴───────────────────╯
```

- Reopen the repository in a container locally.
- Open the repository in a container on Github Codespaces.
  
Follow the Arista Community Central article below for more information:
"Link"
