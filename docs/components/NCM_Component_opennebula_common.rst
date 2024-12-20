#####################################
NCM\::Component\::opennebula - common
#####################################

Types
-----

 - **/software/components/opennebula/opennebula_device_prefix**
 - **/software/components/opennebula/opennebula_vdc_rules**
 - **/software/components/opennebula/opennebula_mysql_db**
    - */software/components/opennebula/opennebula_mysql_db/server*
        - Optional
        - Type: string
    - */software/components/opennebula/opennebula_mysql_db/port*
        - Optional
        - Type: type_port
    - */software/components/opennebula/opennebula_mysql_db/user*
        - Optional
        - Type: string
    - */software/components/opennebula/opennebula_mysql_db/passwd*
        - Optional
        - Type: string
    - */software/components/opennebula/opennebula_mysql_db/db_name*
        - Optional
        - Type: string
    - */software/components/opennebula/opennebula_mysql_db/connections*
        - Description: Number of DB connections. The DB needs to be configured to support oned + monitord connections.
        - Required
        - Type: long
        - Range: 1..
        - Default value: 25
    - */software/components/opennebula/opennebula_mysql_db/compare_binary*
        - Description: Compare strings using BINARY clause makes name searches case sensitive
        - Required
        - Type: boolean
        - Default value: false
 - **/software/components/opennebula/opennebula_db**
    - */software/components/opennebula/opennebula_db/backend*
        - Required
        - Type: string
 - **/software/components/opennebula/opennebula_log**
    - */software/components/opennebula/opennebula_log/system*
        - Description: Configuration for the logging system file: to log in the sched.log file syslog: to use the syslog facilities
        - Required
        - Type: string
        - Default value: file
    - */software/components/opennebula/opennebula_log/debug_level*
        - Description: debug_level: 0 = ERROR 1 = WARNING 2 = INFO 3 = DEBUG Includes general scheduling information (default) 4 = DDEBUG Includes time taken for each step 5 = DDDEBUG Includes detailed information about the scheduling decision, such as VM requirements, Host ranking for each VM, etc. This will impact the performance
        - Required
        - Type: long
        - Range: 0..5
        - Default value: 3
 - **/software/components/opennebula/opennebula_im**
    - */software/components/opennebula/opennebula_im/name*
        - Required
        - Type: string
    - */software/components/opennebula/opennebula_im/executable*
        - Required
        - Type: string
        - Default value: one_im_ssh
    - */software/components/opennebula/opennebula_im/arguments*
        - Required
        - Type: string
    - */software/components/opennebula/opennebula_im/sunstone_name*
        - Optional
        - Type: string
    - */software/components/opennebula/opennebula_im/threads*
        - Description: Number of threads, i.e. number of hosts monitored at the same time
        - Optional
        - Type: long
        - Range: 0..
 - **/software/components/opennebula/opennebula_vm**
    - */software/components/opennebula/opennebula_vm/executable*
        - Required
        - Type: string
        - Default value: one_vmm_exec
    - */software/components/opennebula/opennebula_vm/arguments*
        - Required
        - Type: string
    - */software/components/opennebula/opennebula_vm/default*
        - Required
        - Type: string
    - */software/components/opennebula/opennebula_vm/sunstone_name*
        - Required
        - Type: string
    - */software/components/opennebula/opennebula_vm/imported_vms_actions*
        - Required
        - Type: string
    - */software/components/opennebula/opennebula_vm/keep_snapshots*
        - Required
        - Type: boolean
        - Default value: true
 - **/software/components/opennebula/opennebula_rpc_service**
    - Description: type for opennebula service common RPC attributes.
    - */software/components/opennebula/opennebula_rpc_service/one_xmlrpc*
        - Description: OpenNebula daemon RPC contact information
        - Required
        - Type: type_absoluteURI
        - Default value: http://localhost:2633/RPC2
    - */software/components/opennebula/opennebula_rpc_service/core_auth*
        - Description: authentication driver to communicate with OpenNebula core
        - Required
        - Type: string
        - Default value: cipher

Functions
---------

 - is_consistent_database
    - Description: check if a specific type of database has the right attributes
 - is_consistent_datastore
    - Description: check if a specific type of datastore has the right attributes
 - is_consistent_vnet
    - Description: check if a specific type of vnet has the right attributes
