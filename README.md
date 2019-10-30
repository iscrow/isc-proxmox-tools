# isc-proxmox-tools
A collection of tools that helps me run my proxmox clusters

### pve_replicate
Replicates **the latest vzdump backup for each vm** between file storage destinations. You can run it nightly and copy them to one destination for a nightly replica and weekly to another destination for a weekly replica.

### pve_run_on_single_node
It will run whatever a command passed as parameter only on a single **quorate** node in a cluster. Say you need something to run only once for the whole cluster from a single one of the nodes. You can schedule it to run on all of them and only one will execute it as long as it's quotrate. That way if the node that usually runs it fails, another will run it next time.


