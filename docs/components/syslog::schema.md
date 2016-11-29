### Types

- `/software/syslog/component_selector_type`
    - `/software/syslog/component_selector_type/facility`
        - required
        - type: string
    - `/software/syslog/component_selector_type/priority`
        - required
        - type: string
- `/software/syslog/component_syslog_type`
    - `/software/syslog/component_syslog_type/selector`
        - optional
        - type: component_selector_type
    - `/software/syslog/component_syslog_type/action`
        - required
        - type: string
    - `/software/syslog/component_syslog_type/template`
        - optional
        - type: string
    - `/software/syslog/component_syslog_type/comment`
        - optional
        - type: string
- `/software/syslog/component_syslog_entries`
    - `/software/syslog/component_syslog_entries/config`
        - required
        - type: component_syslog_type
    - `/software/syslog/component_syslog_entries/directives`
        - optional
        - type: string
    - `/software/syslog/component_syslog_entries/daemontype`
        - optional
        - type: string
    - `/software/syslog/component_syslog_entries/file`
        - optional
        - type: string
    - `/software/syslog/component_syslog_entries/syslogdoptions`
        - optional
        - type: string
    - `/software/syslog/component_syslog_entries/klogdoptions`
        - optional
        - type: string
    - `/software/syslog/component_syslog_entries/fullcontrol`
        - optional
        - type: boolean
