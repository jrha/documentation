
### Types

 - `/software/postgresql/postgresql_hba_database`
 - `/software/postgresql/postgresql_hba_user`
 - `/software/postgresql/postgresql_hba`
    - `/software/postgresql/postgresql_hba/host`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_hba/database`
        - Optional
        - Type: postgresql_hba_database
    - `/software/postgresql/postgresql_hba/user`
        - Optional
        - Type: postgresql_hba_user
    - `/software/postgresql/postgresql_hba/address`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_hba/method`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_hba/options`
        - Optional
        - Type: string
 - `/software/postgresql/postgresql_mainconfig`
    - Description: 
    postgresql main configuration
        boolean -> yes / no
        int     -> int
        string  -> 'string' (use double single quotes for a single quote in the string)

    - `/software/postgresql/postgresql_mainconfig/archive_command`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/archive_mode`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/archive_timeout`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/array_nulls`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/authentication_timeout`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/autovacuum`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/autovacuum_analyze_scale_factor`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/autovacuum_analyze_threshold`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/autovacuum_freeze_max_age`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/autovacuum_max_workers`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/autovacuum_naptime`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/autovacuum_vacuum_cost_delay`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/autovacuum_vacuum_cost_limit`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/autovacuum_vacuum_scale_factor`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/autovacuum_vacuum_threshold`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/backslash_quote`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/bgwriter_delay`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/bgwriter_lru_maxpages`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/bgwriter_lru_multiplier`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/bonjour`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/bonjour_name`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/bytea_output`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/check_function_bodies`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/checkpoint_completion_target`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/checkpoint_segments`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/checkpoint_timeout`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/checkpoint_warning`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/client_encoding`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/client_min_messages`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/commit_delay`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/commit_siblings`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/constraint_exclusion`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/cpu_index_tuple_cost`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/cpu_operator_cost`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/cpu_tuple_cost`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/cursor_tuple_fraction`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/custom_variable_classes`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/data_directory`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/datestyle`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/db_user_namespace`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/deadlock_timeout`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/debug_pretty_print`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/debug_print_parse`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/debug_print_plan`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/debug_print_rewritten`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/default_statistics_target`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/default_tablespace`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/default_text_search_config`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/default_transaction_deferrable`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/default_transaction_isolation`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/default_transaction_read_only`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/default_with_oids`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/dynamic_library_path`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/effective_cache_size`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/effective_io_concurrency`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/enable_bitmapscan`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/enable_hashagg`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/enable_hashjoin`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/enable_indexscan`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/enable_material`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/enable_mergejoin`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/enable_nestloop`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/enable_seqscan`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/enable_sort`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/enable_tidscan`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/escape_string_warning`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/exit_on_error`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/external_pid_file`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/extra_float_digits`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/from_collapse_limit`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/fsync`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/full_page_writes`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/geqo`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/geqo_effort`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/geqo_generations`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/geqo_pool_size`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/geqo_seed`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/geqo_selection_bias`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/geqo_threshold`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/hba_file`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/hot_standby`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/hot_standby_feedback`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/ident_file`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/intervalstyle`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/join_collapse_limit`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/krb_caseins_users`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/krb_server_keyfile`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/krb_srvname`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/lc_messages`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/lc_monetary`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/lc_numeric`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/lc_time`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/listen_addresses`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/lo_compat_privileges`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/local_preload_libraries`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/log_autovacuum_min_duration`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/log_checkpoints`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/log_connections`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/log_destination`
        - Optional
        - Type: string
        - Default value: stderr
    - `/software/postgresql/postgresql_mainconfig/log_directory`
        - Optional
        - Type: string
        - Default value: pg_log
    - `/software/postgresql/postgresql_mainconfig/log_disconnections`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/log_duration`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/log_error_verbosity`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/log_executor_stats`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/log_file_mode`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/log_filename`
        - Optional
        - Type: string
        - Default value: postgresql-%a.log
    - `/software/postgresql/postgresql_mainconfig/log_hostname`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/log_line_prefix`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/log_lock_waits`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/log_min_duration_statement`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/log_min_error_statement`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/log_min_messages`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/log_parser_stats`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/log_planner_stats`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/log_rotation_age`
        - Optional
        - Type: string
        - Default value: 1d
    - `/software/postgresql/postgresql_mainconfig/log_rotation_size`
        - Optional
        - Type: long
        - Default value: 0
    - `/software/postgresql/postgresql_mainconfig/log_statement`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/log_statement_stats`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/log_temp_files`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/log_timezone`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/log_truncate_on_rotation`
        - Optional
        - Type: boolean
        - Default value: true
    - `/software/postgresql/postgresql_mainconfig/logging_collector`
        - Optional
        - Type: boolean
        - Default value: true
    - `/software/postgresql/postgresql_mainconfig/maintenance_work_mem`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/max_connections`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/max_files_per_process`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/max_locks_per_transaction`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/max_pred_locks_per_transaction`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/max_prepared_transactions`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/max_stack_depth`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/max_standby_archive_delay`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/max_standby_streaming_delay`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/max_wal_senders`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/password_encryption`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/port`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/quote_all_identifiers`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/random_page_cost`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/replication_timeout`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/restart_after_crash`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/search_path`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/seq_page_cost`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/session_replication_role`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/shared_buffers`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/shared_preload_libraries`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/silent_mode`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/sql_inheritance`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/ssl`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/ssl_ciphers`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/ssl_renegotiation_limit`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/standard_conforming_strings`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/statement_timeout`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/stats_temp_directory`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/superuser_reserved_connections`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/synchronize_seqscans`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/synchronous_commit`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/synchronous_standby_names`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/syslog_facility`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/syslog_ident`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/tcp_keepalives_count`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/tcp_keepalives_idle`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/tcp_keepalives_interval`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/temp_buffers`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/temp_tablespaces`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/timezone`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/timezone_abbreviations`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/track_activities`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/track_activity_query_size`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/track_counts`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/track_functions`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/transform_null_equals`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/unix_socket_directory`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/unix_socket_group`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/unix_socket_permissions`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/update_process_title`
        - Optional
        - Type: boolean
    - `/software/postgresql/postgresql_mainconfig/vacuum_cost_delay`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/vacuum_cost_limit`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/vacuum_cost_page_dirty`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/vacuum_cost_page_hit`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/vacuum_cost_page_miss`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/vacuum_defer_cleanup_age`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/vacuum_freeze_min_age`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/vacuum_freeze_table_age`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/wal_buffers`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/wal_keep_segments`
        - Optional
        - Type: long
    - `/software/postgresql/postgresql_mainconfig/wal_level`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/wal_receiver_status_interval`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/wal_sender_delay`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/wal_sync_method`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/wal_writer_delay`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/work_mem`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/xmlbinary`
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_mainconfig/xmloption`
        - Optional
        - Type: string
 - `/software/postgresql/postgresql_db`
    - `/software/postgresql/postgresql_db/installfile`
        - Description: this file is used to initialise the database (using the pgsql -f option)
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_db/lang`
        - Description: sets the pg language for the db (using createlang), this runs after installfile. 
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_db/langfile`
        - Description: this file is used to add procedures in certain lang (using pgsql -f option), this runs after successful lang is added
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_db/sql_user`
        - Description: apply the installfile with this user (if not defined, the owner is used)
        - Optional
        - Type: string
    - `/software/postgresql/postgresql_db/user`
        - Description: database owner
        - Optional
        - Type: string
 - `/software/postgresql/postgresql_config`
    - `/software/postgresql/postgresql_config/hba`
        - Optional
        - Type: postgresql_hba
    - `/software/postgresql/postgresql_config/main`
        - Optional
        - Type: postgresql_mainconfig
    - `/software/postgresql/postgresql_config/debug_print`
        - Optional
        - Type: long
 - `/software/postgresql/postgresql_role_sql`
    - Description: 
    The raw ALTER ROLE sql (cannot contain a ';'; use ENCRYPTED PASSWORD instead)

 - `/software/postgresql/component_postgresql`
    - `/software/postgresql/component_postgresql/commands`
        - Optional
        - Type: string
    - `/software/postgresql/component_postgresql/config`
        - Optional
        - Type: postgresql_config
    - `/software/postgresql/component_postgresql/databases`
        - Description: Databases are only added/created, never updated, modified or removed.
        - Optional
        - Type: postgresql_db
    - `/software/postgresql/component_postgresql/pg_dir`
        - Optional
        - Type: string
    - `/software/postgresql/component_postgresql/pg_engine`
        - Optional
        - Type: string
    - `/software/postgresql/component_postgresql/pg_hba`
        - Optional
        - Type: string
    - `/software/postgresql/component_postgresql/pg_port`
        - Optional
        - Type: string
    - `/software/postgresql/component_postgresql/pg_script_name`
        - Optional
        - Type: string
    - `/software/postgresql/component_postgresql/pg_version`
        - Optional
        - Type: string
    - `/software/postgresql/component_postgresql/postgresql_conf`
        - Optional
        - Type: string
    - `/software/postgresql/component_postgresql/roles`
        - Description: role name with ROLE ALTER SQL command. Roles are only added and updated, never removed.
        - Optional
        - Type: postgresql_role_sql

### Functions

 - postgresql_is_hba_db
 - postgresql_is_hba_address
