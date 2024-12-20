#########################################################
NCM\::Component\::metaconfig\::elasticsearch - schema_8.1
#########################################################

Types
-----

 - **/software/components/metaconfig/elasticsearch_bootstrap**
    - Description: version specific types for Elasticsearch version 8.1 and later
    - */software/components/metaconfig/elasticsearch_bootstrap/memory_lock*
        - Optional
        - Type: boolean
 - **/software/components/metaconfig/elasticsearch_path**
    - */software/components/metaconfig/elasticsearch_path/repo*
        - Optional
        - Type: absolute_file_path
    - */software/components/metaconfig/elasticsearch_path/data*
        - Required
        - Type: absolute_file_path
    - */software/components/metaconfig/elasticsearch_path/logs*
        - Required
        - Type: absolute_file_path
 - **/software/components/metaconfig/elasticsearch_thread_pool_fixed**
    - Description: fixed thread pool
    - */software/components/metaconfig/elasticsearch_thread_pool_fixed/size*
        - Optional
        - Type: long
        - Range: 0..
    - */software/components/metaconfig/elasticsearch_thread_pool_fixed/queue_size*
        - Optional
        - Type: long
        - Range: -1..
 - **/software/components/metaconfig/elasticsearch_thread_pool_scaling**
    - Description: scaling thread pool
    - */software/components/metaconfig/elasticsearch_thread_pool_scaling/core*
        - Optional
        - Type: long
        - Range: 1..
    - */software/components/metaconfig/elasticsearch_thread_pool_scaling/max*
        - Optional
        - Type: long
        - Range: 1..
    - */software/components/metaconfig/elasticsearch_thread_pool_scaling/keep_alive*
        - Description: time in seconds to keep idle thread in thread pool
        - Optional
        - Type: long
        - Range: 0..
 - **/software/components/metaconfig/elasticsearch_threadpool**
    - Description: Thread pool management. See http://www.elasticsearch.org/guide/reference/modules/threadpool/ @
    - */software/components/metaconfig/elasticsearch_threadpool/generic*
        - Optional
        - Type: elasticsearch_thread_pool_scaling
    - */software/components/metaconfig/elasticsearch_threadpool/search*
        - Optional
        - Type: elasticsearch_thread_pool_fixed
    - */software/components/metaconfig/elasticsearch_threadpool/index*
        - Optional
        - Type: elasticsearch_thread_pool_fixed
    - */software/components/metaconfig/elasticsearch_threadpool/get*
        - Optional
        - Type: elasticsearch_thread_pool_fixed
    - */software/components/metaconfig/elasticsearch_threadpool/write*
        - Optional
        - Type: elasticsearch_thread_pool_fixed
    - */software/components/metaconfig/elasticsearch_threadpool/snapshot*
        - Optional
        - Type: elasticsearch_thread_pool_scaling
    - */software/components/metaconfig/elasticsearch_threadpool/warmer*
        - Optional
        - Type: elasticsearch_thread_pool_scaling
    - */software/components/metaconfig/elasticsearch_threadpool/refresh*
        - Optional
        - Type: elasticsearch_thread_pool_scaling
    - */software/components/metaconfig/elasticsearch_threadpool/listener*
        - Optional
        - Type: elasticsearch_thread_pool_scaling
 - **/software/components/metaconfig/elasticsearch_xpack_transport_ssl**
    - */software/components/metaconfig/elasticsearch_xpack_transport_ssl/enabled*
        - Required
        - Type: boolean
    - */software/components/metaconfig/elasticsearch_xpack_transport_ssl/key*
        - Required
        - Type: string
    - */software/components/metaconfig/elasticsearch_xpack_transport_ssl/certificate*
        - Required
        - Type: string
    - */software/components/metaconfig/elasticsearch_xpack_transport_ssl/verification_mode*
        - Required
        - Type: string
    - */software/components/metaconfig/elasticsearch_xpack_transport_ssl/certificate_authorities*
        - Required
        - Type: absolute_file_path
 - **/software/components/metaconfig/elasticsearch_xpack_transport**
    - */software/components/metaconfig/elasticsearch_xpack_transport/ssl*
        - Required
        - Type: elasticsearch_xpack_transport_ssl
 - **/software/components/metaconfig/elasticsearch_xpack_http_ssl**
    - */software/components/metaconfig/elasticsearch_xpack_http_ssl/enabled*
        - Required
        - Type: boolean
    - */software/components/metaconfig/elasticsearch_xpack_http_ssl/key*
        - Required
        - Type: string
    - */software/components/metaconfig/elasticsearch_xpack_http_ssl/certificate*
        - Required
        - Type: string
    - */software/components/metaconfig/elasticsearch_xpack_http_ssl/verification_mode*
        - Required
        - Type: string
    - */software/components/metaconfig/elasticsearch_xpack_http_ssl/certificate_authorities*
        - Required
        - Type: absolute_file_path
 - **/software/components/metaconfig/elasticsearch_xpack_http**
    - */software/components/metaconfig/elasticsearch_xpack_http/ssl*
        - Required
        - Type: elasticsearch_xpack_http_ssl
 - **/software/components/metaconfig/elasticsearch_xpack_security**
    - */software/components/metaconfig/elasticsearch_xpack_security/enabled*
        - Required
        - Type: boolean
    - */software/components/metaconfig/elasticsearch_xpack_security/transport*
        - Required
        - Type: elasticsearch_xpack_transport
    - */software/components/metaconfig/elasticsearch_xpack_security/http*
        - Required
        - Type: elasticsearch_xpack_http
 - **/software/components/metaconfig/elasticsearch_xpack**
    - */software/components/metaconfig/elasticsearch_xpack/security*
        - Required
        - Type: elasticsearch_xpack_security
 - **/software/components/metaconfig/elasticsearch_service**
    - */software/components/metaconfig/elasticsearch_service/node*
        - Optional
        - Type: elasticsearch_node
    - */software/components/metaconfig/elasticsearch_service/index*
        - Optional
        - Type: elasticsearch_index
    - */software/components/metaconfig/elasticsearch_service/gateway*
        - Optional
        - Type: elasticsearch_gw
    - */software/components/metaconfig/elasticsearch_service/indices*
        - Optional
        - Type: elasticsearch_indices
    - */software/components/metaconfig/elasticsearch_service/network*
        - Required
        - Type: elasticsearch_network
    - */software/components/metaconfig/elasticsearch_service/monitor.jvm.gc*
        - Required
        - Type: elasticsearch_monitoring
    - */software/components/metaconfig/elasticsearch_service/thread_pool*
        - Optional
        - Type: elasticsearch_threadpool
    - */software/components/metaconfig/elasticsearch_service/bootstrap*
        - Optional
        - Type: elasticsearch_bootstrap
    - */software/components/metaconfig/elasticsearch_service/cluster*
        - Optional
        - Type: elasticsearch_cluster
    - */software/components/metaconfig/elasticsearch_service/transport*
        - Optional
        - Type: elasticsearch_transport
    - */software/components/metaconfig/elasticsearch_service/discovery*
        - Optional
        - Type: elasticsearch_discovery
    - */software/components/metaconfig/elasticsearch_service/path*
        - Required
        - Type: elasticsearch_path
    - */software/components/metaconfig/elasticsearch_service/processors*
        - Optional
        - Type: long
        - Range: 1..
    - */software/components/metaconfig/elasticsearch_service/xpack*
        - Optional
        - Type: elasticsearch_xpack
