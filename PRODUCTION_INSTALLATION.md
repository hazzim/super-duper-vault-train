# Use for Production Installation

If you want to install this in a production cluster, run the [`*.sh` scripts named inside the Vagrantfile](https://github.com/v6/super-duper-vault-train/blob/develop/Vagrantfile#L22-L36) in the order that they're listed, on each host, using the arguments listed as bash arguments. 

For example, for [`server.vm.provision "shell", path: "account.sh", args: "consul-replicate"`](https://github.com/v6/super-duper-vault-train/blob/develop/Vagrantfile#L24), you would run `# account.sh consul-replicate` as root.

After running `# account.sh consul-replicate`, you would run the next listed `.sh` file, `prereqs.sh`, and so on.