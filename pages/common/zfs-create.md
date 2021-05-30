# zfs create

> Create ZFS filesystems

- Create a basic filesystem that will be in the root of the pool:

`zfs create {{pool_name/filesystem_name}}`

- Create a filesystem that will mount in a specific directory:

`zfs create -o mountpoint=/path/to/mountpoint {{pool_name/filesystem_name}}`

- Create a filesystem with compression enabled:

`zfs create -o compression=on {{pool_name/filesystem_name}}`

- Create a filesystem with a quota (a size limit), for example, for a 10 GB filesystem:

`zfs create -o quota=10G {{pool_name/filesystem_name}}`

- When you create ZFS filesystems, you can also create them in another filesystem:

`zfs create {{pool_name/existing_filesystem_name/new_filesystem_name}}


