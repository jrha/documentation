##############################################
NCM\::Component\::metaconfig\::xinetd - schema
##############################################

Types
-----

 - **/software/components/metaconfig/xinetd_options_type**
 - **/software/components/metaconfig/xinetd_options_flags**
 - **/software/components/metaconfig/xinetd_options_ips**
 - **/software/components/metaconfig/xinetd_options_log_on_success**
 - **/software/components/metaconfig/xinetd_options_log_on_failure**
 - **/software/components/metaconfig/xinetd_options**
    - */software/components/metaconfig/xinetd_options/disable*
        - Required
        - Type: boolean
        - Default value: false
    - */software/components/metaconfig/xinetd_options/wait*
        - Required
        - Type: boolean
        - Default value: true
    - */software/components/metaconfig/xinetd_options/id*
        - Optional
        - Type: string
    - */software/components/metaconfig/xinetd_options/type*
        - Optional
        - Type: xinetd_options_type
    - */software/components/metaconfig/xinetd_options/flags*
        - Optional
        - Type: xinetd_options_flags
    - */software/components/metaconfig/xinetd_options/only_from*
        - Optional
        - Type: xinetd_options_ips
    - */software/components/metaconfig/xinetd_options/cps*
        - Optional
        - Type: long
    - */software/components/metaconfig/xinetd_options/port*
        - Optional
        - Type: long
        - Range: 0..
    - */software/components/metaconfig/xinetd_options/socket_type*
        - Required
        - Type: choice
    - */software/components/metaconfig/xinetd_options/user*
        - Required
        - Type: string
        - Default value: root
    - */software/components/metaconfig/xinetd_options/server*
        - Optional
        - Type: string
    - */software/components/metaconfig/xinetd_options/protocol*
        - Optional
        - Type: choice
    - */software/components/metaconfig/xinetd_options/server_args*
        - Optional
        - Type: string
    - */software/components/metaconfig/xinetd_options/group*
        - Optional
        - Type: string
    - */software/components/metaconfig/xinetd_options/instances*
        - Optional
        - Type: string
    - */software/components/metaconfig/xinetd_options/per_source*
        - Optional
        - Type: long
    - */software/components/metaconfig/xinetd_options/log_on_success*
        - Optional
        - Type: xinetd_options_log_on_success
    - */software/components/metaconfig/xinetd_options/log_on_failure*
        - Optional
        - Type: xinetd_options_log_on_failure
 - **/software/components/metaconfig/xinetd_conf**
    - */software/components/metaconfig/xinetd_conf/servicename*
        - Required
        - Type: string
    - */software/components/metaconfig/xinetd_conf/options*
        - Required
        - Type: xinetd_options
