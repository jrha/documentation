
### Types

 - `/software/gpfs/component_gpfs_cfg`
    - `/software/gpfs/component_gpfs_cfg/url`
        - Optional
        - Type: string
    - `/software/gpfs/component_gpfs_cfg/keyData`
        - Optional
        - Type: string
    - `/software/gpfs/component_gpfs_cfg/sdrrestore`
        - Optional
        - Type: boolean
        - Default value: false
    - `/software/gpfs/component_gpfs_cfg/subnet`
        - Optional
        - Type: string
    - `/software/gpfs/component_gpfs_cfg/usecurl`
        - Optional
        - Type: boolean
        - Default value: true
    - `/software/gpfs/component_gpfs_cfg/useccmcertwithcurl`
        - Optional
        - Type: boolean
        - Default value: false
    - `/software/gpfs/component_gpfs_cfg/usesindesgetcertcertwithcurl`
        - Optional
        - Type: boolean
        - Default value: false
 - `/software/gpfs/component_gpfs_base`
    - `/software/gpfs/component_gpfs_base/rpms`
        - Optional
        - Type: string
    - `/software/gpfs/component_gpfs_base/baseurl`
        - Optional
        - Type: string
    - `/software/gpfs/component_gpfs_base/useproxy`
        - Optional
        - Type: boolean
        - Default value: false
    - `/software/gpfs/component_gpfs_base/usecurl`
        - Optional
        - Type: boolean
        - Default value: false
    - `/software/gpfs/component_gpfs_base/useccmcertwithcurl`
        - Optional
        - Type: boolean
        - Default value: false
    - `/software/gpfs/component_gpfs_base/usesindesgetcertcertwithcurl`
        - Optional
        - Type: boolean
        - Default value: false
    - `/software/gpfs/component_gpfs_base/useyum`
        - Optional
        - Type: boolean
        - Default value: true
 - `/software/gpfs/component_gpfs`
    - `/software/gpfs/component_gpfs/base`
        - Optional
        - Type: component_gpfs_base
    - `/software/gpfs/component_gpfs/cfg`
        - Optional
        - Type: component_gpfs_cfg
