#######################################
NCM\::Component\::altlogrotate - schema
#######################################

Types
-----

 - **/software/components/altlogrotate/structure_altlogrotate_scripts**
    - */software/components/altlogrotate/structure_altlogrotate_scripts/prerotate*
        - Optional
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_scripts/postrotate*
        - Optional
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_scripts/firstaction*
        - Optional
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_scripts/lastaction*
        - Optional
        - Type: string
 - **/software/components/altlogrotate/structure_altlogrotate_create_params**
    - */software/components/altlogrotate/structure_altlogrotate_create_params/mode*
        - Required
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_create_params/owner*
        - Required
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_create_params/group*
        - Required
        - Type: string
 - **/software/components/altlogrotate/structure_altlogrotate_su**
    - */software/components/altlogrotate/structure_altlogrotate_su/user*
        - Required
        - Type: string_trimmed
    - */software/components/altlogrotate/structure_altlogrotate_su/group*
        - Required
        - Type: string_trimmed
 - **/software/components/altlogrotate/structure_altlogrotate_logrot**
    - */software/components/altlogrotate/structure_altlogrotate_logrot/pattern*
        - Optional
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_logrot/global*
        - Description: part of global configuration file, requires an entry called 'global'. The 'global' entry does not require the global flag.
        - Optional
        - Type: boolean
    - */software/components/altlogrotate/structure_altlogrotate_logrot/overwrite*
        - Description: Create and overwrite configfile with the entry as filename, if it previously existed (only non-global files). (If such file does not exist, use the ncm-altlogrotate suffix as usual)
        - Optional
        - Type: boolean
    - */software/components/altlogrotate/structure_altlogrotate_logrot/include*
        - Optional
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_logrot/compress*
        - Optional
        - Type: boolean
    - */software/components/altlogrotate/structure_altlogrotate_logrot/copy*
        - Optional
        - Type: boolean
    - */software/components/altlogrotate/structure_altlogrotate_logrot/copytruncate*
        - Optional
        - Type: boolean
    - */software/components/altlogrotate/structure_altlogrotate_logrot/delaycompress*
        - Optional
        - Type: boolean
    - */software/components/altlogrotate/structure_altlogrotate_logrot/ifempty*
        - Optional
        - Type: boolean
    - */software/components/altlogrotate/structure_altlogrotate_logrot/missingok*
        - Optional
        - Type: boolean
    - */software/components/altlogrotate/structure_altlogrotate_logrot/sharedscripts*
        - Optional
        - Type: boolean
    - */software/components/altlogrotate/structure_altlogrotate_logrot/dateext*
        - Optional
        - Type: boolean
    - */software/components/altlogrotate/structure_altlogrotate_logrot/compresscmd*
        - Optional
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_logrot/uncompresscmd*
        - Optional
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_logrot/compressext*
        - Optional
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_logrot/compressoptions*
        - Optional
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_logrot/create*
        - Optional
        - Type: boolean
    - */software/components/altlogrotate/structure_altlogrotate_logrot/createparams*
        - Optional
        - Type: structure_altlogrotate_create_params
    - */software/components/altlogrotate/structure_altlogrotate_logrot/extension*
        - Optional
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_logrot/mail*
        - Optional
        - Type: type_email
    - */software/components/altlogrotate/structure_altlogrotate_logrot/nomail*
        - Optional
        - Type: boolean
    - */software/components/altlogrotate/structure_altlogrotate_logrot/mailselect*
        - Optional
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_logrot/olddir*
        - Optional
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_logrot/noolddir*
        - Optional
        - Type: boolean
    - */software/components/altlogrotate/structure_altlogrotate_logrot/rotate*
        - Optional
        - Type: long
        - Range: 0..
    - */software/components/altlogrotate/structure_altlogrotate_logrot/start*
        - Optional
        - Type: long
        - Range: 0..
    - */software/components/altlogrotate/structure_altlogrotate_logrot/size*
        - Optional
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_logrot/taboo_replace*
        - Optional
        - Type: boolean
    - */software/components/altlogrotate/structure_altlogrotate_logrot/tabooext*
        - Optional
        - Type: string
    - */software/components/altlogrotate/structure_altlogrotate_logrot/frequency*
        - Optional
        - Type: choice
    - */software/components/altlogrotate/structure_altlogrotate_logrot/scripts*
        - Optional
        - Type: structure_altlogrotate_scripts
    - */software/components/altlogrotate/structure_altlogrotate_logrot/su*
        - Optional
        - Type: structure_altlogrotate_su
 - **/software/components/altlogrotate/altlogrotate_component**
    - */software/components/altlogrotate/altlogrotate_component/configFile*
        - Description: Logrotate configuration file location, defaults to /etc/logrotate.conf.
        - Required
        - Type: string
        - Default value: /etc/logrotate.conf
    - */software/components/altlogrotate/altlogrotate_component/configDir*
        - Description: Logrotate entries directory path, defaults to /etc/logrotate.d, entries will be written to individual config files under this path.
        - Required
        - Type: string
        - Default value: /etc/logrotate.d
    - */software/components/altlogrotate/altlogrotate_component/entries*
        - Description: A named list containing logrotate structures. Follows the logrotate config format, so see 'man 8 logrotate' for a detailed explanation of all options. The 'global' entry (if exists) is put at the beginning of the main configuration.
        - Required
        - Type: structure_altlogrotate_logrot
