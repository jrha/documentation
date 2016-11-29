### Types

- `/software/pnp4nagios/pnp4nagios_php_view_type`
    - `/software/pnp4nagios/pnp4nagios_php_view_type/title`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_view_type/start`
        - required
        - type: long
- `/software/pnp4nagios/pnp4nagios_npcd_log_type`
- `/software/pnp4nagios/pnp4nagios_php_paper_size`
- `/software/pnp4nagios/pnp4nagios_php_ui_theme`
- `/software/pnp4nagios/pnp4nagios_php_lang`
- `/software/pnp4nagios/pnp4nagios_perfdata_RRD_storage_type`
- `/software/pnp4nagios/pnp4nagios_npcd_config`
    - `/software/pnp4nagios/pnp4nagios_npcd_config/user`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_npcd_config/group`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_npcd_config/log_type`
        - required
        - type: pnp4nagios_npcd_log_type
    - `/software/pnp4nagios/pnp4nagios_npcd_config/log_file`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_npcd_config/max_logfile_size`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_npcd_config/log_level`
        - required
        - type: long
        - range: 0..2
    - `/software/pnp4nagios/pnp4nagios_npcd_config/perfdata_spool_dir`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_npcd_config/perfdata_file_run_cmd`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_npcd_config/perfdata_file_run_cmd_args`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_npcd_config/identify_npcd`
        - required
        - type: boolean
    - `/software/pnp4nagios/pnp4nagios_npcd_config/npcd_max_threads`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_npcd_config/sleep_time`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_npcd_config/load_threshold`
        - required
        - type: double
    - `/software/pnp4nagios/pnp4nagios_npcd_config/pid_file`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_npcd_config/perfdata_file`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_npcd_config/perfdata_spool_filename`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_npcd_config/perfdata_file_processing_interval`
        - required
        - type: long
- `/software/pnp4nagios/pnp4nagios_php_config`
    - `/software/pnp4nagios/pnp4nagios_php_config/use_url_rewriting`
        - required
        - type: boolean
    - `/software/pnp4nagios/pnp4nagios_php_config/rrdtool`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/graph_width`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_php_config/graph_height`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_php_config/zgraph_width`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_php_config/zgraph_height`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_php_config/right_zoom_offset`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_php_config/pdf_width`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_php_config/pdf_height`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_php_config/pdf_page_size`
        - required
        - type: pnp4nagios_php_paper_size
    - `/software/pnp4nagios/pnp4nagios_php_config/pdf_margin_top`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_php_config/pdf_margin_left`
        - required
        - type: double
    - `/software/pnp4nagios/pnp4nagios_php_config/pdf_margin_right`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_php_config/graph_opt`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/pdf_graph_opt`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/rrdbase`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/page_dir`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/refresh`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_php_config/max_age`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_php_config/temp`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/nagios_base`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/multisite_base_url`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/multisite_site`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/auth_enabled`
        - required
        - type: boolean
    - `/software/pnp4nagios/pnp4nagios_php_config/livestatus_socket`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/allowed_for_all_services`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/allowed_for_all_hosts`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/allowed_for_service_links`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/allowed_for_host_search`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/allowed_for_host_overview`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/allowed_for_pages`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/overview`-range
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_php_config/popup`-width
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/ui`-theme
        - required
        - type: pnp4nagios_php_ui_theme
    - `/software/pnp4nagios/pnp4nagios_php_config/lang`
        - required
        - type: pnp4nagios_php_lang
    - `/software/pnp4nagios/pnp4nagios_php_config/date_fmt`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/enable_recursive_template_search`
        - required
        - type: boolean
    - `/software/pnp4nagios/pnp4nagios_php_config/show_xml_icon`
        - required
        - type: boolean
    - `/software/pnp4nagios/pnp4nagios_php_config/use_fpdf`
        - required
        - type: boolean
    - `/software/pnp4nagios/pnp4nagios_php_config/background_pdf`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/use_calendar`
        - required
        - type: boolean
    - `/software/pnp4nagios/pnp4nagios_php_config/views`
        - required
        - type: pnp4nagios_php_view_type
    - `/software/pnp4nagios/pnp4nagios_php_config/rrd_daemon_opts`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/template_dirs`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/special_template_dir`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_php_config/mobile_devices`
        - required
        - type: string
- `/software/pnp4nagios/pnp4nagios_nagios_config`
    - `/software/pnp4nagios/pnp4nagios_nagios_config/process_performance_data`
        - required
        - type: boolean
    - `/software/pnp4nagios/pnp4nagios_nagios_config/service_perfdata_command`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_nagios_config/process_performance_data`
        - required
        - type: boolean
    - `/software/pnp4nagios/pnp4nagios_nagios_config/service_perfdata_file`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_nagios_config/service_perfdata_file_template`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_nagios_config/service_perfdata_file_mode`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_nagios_config/service_perfdata_file_processing_interval`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_nagios_config/service_perfdata_file_processing_command`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_nagios_config/host_perfdata_file`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_nagios_config/host_perfdata_file_template`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_nagios_config/host_perfdata_file_mode`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_nagios_config/host_perfdata_file_processing_interval`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_nagios_config/host_perfdata_file_processing_command`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_nagios_config/process_performance_data`
        - required
        - type: boolean
    - `/software/pnp4nagios/pnp4nagios_nagios_config/broker_module`
        - required
        - type: string
- `/software/pnp4nagios/pnp4nagios_perfdata_config`
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/timeout`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/use_rrds`
        - required
        - type: boolean
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/rrdpath`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/rrdtool`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/cfg_dir`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/rrd_storage_type`
        - required
        - type: pnp4nagios_perfdata_RRD_storage_type
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/rrd_heartbeat`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/rra_cfg`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/rra_step`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/log_file`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/log_level`
        - required
        - type: long
        - range: 0..2
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/xml_enc`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/xml_update_delay`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/rrd_daemon_opts`
        - optional
        - type: string
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/stats_dir`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/prefork`
        - required
        - type: boolean
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/gearman_host`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/requests_per_child`
        - required
        - type: long
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/encryption`
        - required
        - type: boolean
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/key`
        - required
        - type: string
    - `/software/pnp4nagios/pnp4nagios_perfdata_config/key_file`
        - optional
        - type: string
- `/software/pnp4nagios/structure_component_pnp4nagios`
    - `/software/pnp4nagios/structure_component_pnp4nagios/npcd`
        - required
        - type: pnp4nagios_npcd_config
    - `/software/pnp4nagios/structure_component_pnp4nagios/php`
        - required
        - type: pnp4nagios_php_config
    - `/software/pnp4nagios/structure_component_pnp4nagios/perfdata`
        - required
        - type: pnp4nagios_perfdata_config
    - `/software/pnp4nagios/structure_component_pnp4nagios/nagios`
        - required
        - type: pnp4nagios_nagios_config
