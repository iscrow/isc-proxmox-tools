# isc-proxmox-tools
A collection of tools that helps me run my proxmox clusters

### bondmon
Shows a realtime view of your bond interface states from /proc/net/bonding/bond\*.

### bondview
Shows the state of a particular bond.

### cephmon
Shows a realtime view of the ceph cluster and bond interfaces state.

### ceph-start
Start a ceph cluster stopped with **ceph-stop**.

### ceph-stop
Stop a ceph cluster so cluster can be shutdown. Start back up **with ceph-start**.

### pve_replicate
Replicates **the latest vzdump backup for each vm** between file storage destinations. You can run it nightly and copy them to one destination for a nightly replica and weekly to another destination for a weekly replica.

### pve_run_on_single_node
It will run whatever a command passed as parameter only on a single **quorate** node in a cluster. Say you need something to run only once for the whole cluster from a single one of the nodes. You can schedule it to run on all of them and only one will execute it as long as it's quotrate. That way if the node that usually runs it fails, another will run it next time.


