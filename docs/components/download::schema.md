### Types

- `/software/download/component_download_file`
    - decription: command (no options) to run after download, the filename is added as first and (only) argument
    - decription: Don't consider the remote file to be new until it is this number of minutes old
    - decription: seconds, overrides setting in component
    - `/software/download/component_download_file/href`
        - required
        - type: string
    - `/software/download/component_download_file/post`
        - optional
        - type: string
    - `/software/download/component_download_file/proxy`
        - required
        - type: boolean
    - `/software/download/component_download_file/gssapi`
        - optional
        - type: boolean
    - `/software/download/component_download_file/perm`
        - optional
        - type: string
    - `/software/download/component_download_file/owner`
        - optional
        - type: string
    - `/software/download/component_download_file/group`
        - optional
        - type: string
    - `/software/download/component_download_file/min_age`
        - required
        - type: long
    - `/software/download/component_download_file/cacert`
        - optional
        - type: string
    - `/software/download/component_download_file/capath`
        - optional
        - type: string
    - `/software/download/component_download_file/cert`
        - optional
        - type: string
    - `/software/download/component_download_file/key`
        - optional
        - type: string
    - `/software/download/component_download_file/timeout`
        - optional
        - type: long
- `/software/download/component_download_type`
    - decription: seconds, timeout for HEAD requests which checks for changes
    - decription: seconds, total timeout for fetch of file, can be overridden per file
    - `/software/download/component_download_type/server`
        - optional
        - type: string
    - `/software/download/component_download_type/proto`
        - optional
        - type: string
    - `/software/download/component_download_type/files`
        - optional
        - type: component_download_file
    - `/software/download/component_download_type/proxyhosts`
        - optional
        - type: string
    - `/software/download/component_download_type/head_timeout`
        - optional
        - type: long
    - `/software/download/component_download_type/timeout`
        - optional
        - type: long
