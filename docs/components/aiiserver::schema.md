### Types

- `/software/aiiserver/structure_aiishellfe`
    - `/software/aiiserver/structure_aiishellfe/cachedir`
        - optional
        - type: string
    - `/software/aiiserver/structure_aiishellfe/ca_dir`
        - optional
        - type: string
    - `/software/aiiserver/structure_aiishellfe/ca_file`
        - optional
        - type: string
    - `/software/aiiserver/structure_aiishellfe/cdburl`
        - required
        - type: type_absoluteURI
    - `/software/aiiserver/structure_aiishellfe/cert_file`
        - optional
        - type: string
    - `/software/aiiserver/structure_aiishellfe/key_file`
        - optional
        - type: string
    - `/software/aiiserver/structure_aiishellfe/lockdir`
        - optional
        - type: string
    - `/software/aiiserver/structure_aiishellfe/logfile`
        - optional
        - type: string
    - `/software/aiiserver/structure_aiishellfe/nbpdir`
        - optional
        - type: string
    - `/software/aiiserver/structure_aiishellfe/noaction`
        - optional
        - type: boolean
    - `/software/aiiserver/structure_aiishellfe/nodhcp`
        - optional
        - type: boolean
    - `/software/aiiserver/structure_aiishellfe/nonbp`
        - optional
        - type: boolean
    - `/software/aiiserver/structure_aiishellfe/noosinstall`
        - optional
        - type: boolean
    - `/software/aiiserver/structure_aiishellfe/osinstalldir`
        - optional
        - type: string
    - `/software/aiiserver/structure_aiishellfe/profile_format`
        - required
        - type: string
    - `/software/aiiserver/structure_aiishellfe/profile_prefix`
        - optional
        - type: string
    - `/software/aiiserver/structure_aiishellfe/use_fqdn`
        - required
        - type: boolean
- `/software/aiiserver/structure_aiidhcp`
    - `/software/aiiserver/structure_aiidhcp/dhcpconf`
        - required
        - type: string
    - `/software/aiiserver/structure_aiidhcp/restartcmd`
        - optional
        - type: string
    - `/software/aiiserver/structure_aiidhcp/norestart`
        - optional
        - type: boolean
- `/software/aiiserver/structure_component_aiiserver`
    - `/software/aiiserver/structure_component_aiiserver/aii`-shellfe
        - required
        - type: structure_aiishellfe
    - `/software/aiiserver/structure_component_aiiserver/aii`-dhcp
        - required
        - type: structure_aiidhcp
