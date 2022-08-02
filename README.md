# git-bash-scripts
Collection of CLI helpers in Windows Git BASH


## srtadm - cluster administration

A tool to manage a group of the same remote machines using CLI input.

usage:

  `srtadm "<command>" <mode> <run_user> <server_prefix> <node_count>`

example using defaults to run the `date` command in `blast` mode:

```bash
srtadm date blast
```

- command: a double quoted string that is passed into a remote BASH interpreter (no default)
- mode: run the command in "batch" or "blast" mode, for sequential or parallel execution (default: batch)
- run_user: remote user for the SSH connection (default: suparious)
- server_prefix: the prefix of the network hostname for the SSH connection (default: lab-node_count)
- node_count: the number of nodes to configure with the "server_prefix" (default: 6)
