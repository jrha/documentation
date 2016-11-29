### Types

- `/software/mkgridmap/structure_mkgridmap_local`
    - `/software/mkgridmap/structure_mkgridmap_local/cert`
        - required
        - type: string
    - `/software/mkgridmap/structure_mkgridmap_local/user`
        - required
        - type: string
- `/software/mkgridmap/structure_mkgridmap_lcmaps`
    - `/software/mkgridmap/structure_mkgridmap_lcmaps/flavor`
        - required
        - type: string
    - `/software/mkgridmap/structure_mkgridmap_lcmaps/gridmapfile`
        - required
        - type: string
    - `/software/mkgridmap/structure_mkgridmap_lcmaps/groupmapfile`
        - required
        - type: string
- `/software/mkgridmap/mkgridmap_component_entry`
    - `/software/mkgridmap/mkgridmap_component_entry/mkgridmapconf`
        - required
        - type: string
    - `/software/mkgridmap/mkgridmap_component_entry/format`
        - required
        - type: string
    - `/software/mkgridmap/mkgridmap_component_entry/command`
        - optional
        - type: string
    - `/software/mkgridmap/mkgridmap_component_entry/lcuser`
        - optional
        - type: string
    - `/software/mkgridmap/mkgridmap_component_entry/allow`
        - optional
        - type: string
    - `/software/mkgridmap/mkgridmap_component_entry/deny`
        - optional
        - type: string
    - `/software/mkgridmap/mkgridmap_component_entry/overwrite`
        - required
        - type: boolean
    - `/software/mkgridmap/mkgridmap_component_entry/authURIs`
        - optional
        - type: type_hostURI
    - `/software/mkgridmap/mkgridmap_component_entry/locals`
        - optional
        - type: structure_mkgridmap_local
- `/software/mkgridmap/mkgridmap_component`
    - `/software/mkgridmap/mkgridmap_component/entries`
        - required
        - type: mkgridmap_component_entry
    - `/software/mkgridmap/mkgridmap_component/lcmaps`
        - optional
        - type: structure_mkgridmap_lcmaps
    - `/software/mkgridmap/mkgridmap_component/voList`
        - optional
        - type: string
