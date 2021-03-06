
### Types

 - `/software/autofs/autofs_conf_common`
 - `/software/autofs/autofs_conf_autofs`
    - `/software/autofs/autofs_conf_autofs/timeout`
        - Optional
        - Type: long
        - Range: 0..
    - `/software/autofs/autofs_conf_autofs/negative_timeout`
        - Optional
        - Type: long
        - Range: 0..
    - `/software/autofs/autofs_conf_autofs/mount_wait`
        - Optional
        - Type: long
        - Range: 0..
    - `/software/autofs/autofs_conf_autofs/umount_wait`
        - Optional
        - Type: long
        - Range: 0..
    - `/software/autofs/autofs_conf_autofs/browse_mode`
        - Optional
        - Type: boolean
    - `/software/autofs/autofs_conf_autofs/append_options`
        - Optional
        - Type: boolean
    - `/software/autofs/autofs_conf_autofs/logging`
        - Optional
        - Type: string
 - `/software/autofs/autofs_conf_amd`
    - `/software/autofs/autofs_conf_amd/dismount_interval`
        - Optional
        - Type: long
        - Range: 0..
    - `/software/autofs/autofs_conf_amd/map_type`
        - Optional
        - Type: string
    - `/software/autofs/autofs_conf_amd/autofs_use_lofs`
        - Optional
        - Type: boolean
 - `/software/autofs/autofs_conf`
    - `/software/autofs/autofs_conf/autofs`
        - Optional
        - Type: autofs_conf_autofs
    - `/software/autofs/autofs_conf/amd`
        - Optional
        - Type: autofs_conf_amd
    - `/software/autofs/autofs_conf/mountpoints`
        - Optional
        - Type: autofs_conf_amd
 - `/software/autofs/autofs_mapentry_type`
    - `/software/autofs/autofs_mapentry_type/options`
        - Description: Specific mount options to be used with this entry.
        - Optional
        - Type: string
    - `/software/autofs/autofs_mapentry_type/location`
        - Description: NFS server name/path associated with this entry.
        - Optional
        - Type: string
 - `/software/autofs/autofs_map_type`
    - `/software/autofs/autofs_map_type/enabled`
        - Description: If false, ignore entries for this map (no change made).
        - Optional
        - Type: boolean
        - Default value: true
    - `/software/autofs/autofs_map_type/preserve`
        - Description: This flag indicated if local changes to the map must be
      preserved (true) or not (false).
        - Optional
        - Type: boolean
        - Default value: true
    - `/software/autofs/autofs_map_type/type`
        - Description: Map type. Supported types are : direct, file, program, yp, nisplus, hesiod, userdir and ldap.
      Only direct, file and program map contents can be managed by this component.
        - Optional
        - Type: string
    - `/software/autofs/autofs_map_type/mapname`
        - Description: Map name. If not defined, a default name is build (/etc/auto suffixed by map entry name).
        - Optional
        - Type: string
    - `/software/autofs/autofs_map_type/mountpoint`
        - Description: Mount point associated with this map.
        - Optional
        - Type: string
    - `/software/autofs/autofs_map_type/mpaliases`
        - Description: mount point aliases (deprecated)
        - Optional
        - Type: string
    - `/software/autofs/autofs_map_type/options`
        - Description: Mount options to be used with this map.
        - Optional
        - Type: string
    - `/software/autofs/autofs_map_type/entries`
        - Description: One entry per filesystem to mount. The key is used to build the mount point. The actual
    mount point depends on map type.
        - Optional
        - Type: autofs_mapentry_type
 - `/software/autofs/autofs_component`
    - `/software/autofs/autofs_component/preserveMaster`
        - Description: This flag indicated if local changes to master map
      must be preserved (true) or not (false).
        - Optional
        - Type: boolean
        - Default value: true
    - `/software/autofs/autofs_component/maps`
        - Description: This resource contains one entry per autofs map to manage. The dict key is
    mainly an internal name but it will be used to build the default map name.
        - Optional
        - Type: autofs_map_type
    - `/software/autofs/autofs_component/conf`
        - Optional
        - Type: autofs_conf
