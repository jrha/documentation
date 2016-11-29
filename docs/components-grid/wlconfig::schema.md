### Types

- `/software/wlconfig/structure_wl_log`
    - `/software/wlconfig/structure_wl_log/file`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_log/level`
        - required
        - type: long
        - range: 1..
- `/software/wlconfig/structure_wl_jobcontroller`
    - `/software/wlconfig/structure_wl_jobcontroller/condorSubmit`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_jobcontroller/condorRemove`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_jobcontroller/condorQuery`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_jobcontroller/condorSubmitDAG`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_jobcontroller/condorRelease`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_jobcontroller/container`
        - required
        - type: long
    - `/software/wlconfig/structure_wl_jobcontroller/submitFile`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_jobcontroller/outputFile`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_jobcontroller/queueFile`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_jobcontroller/lockFile`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_jobcontroller/log`
        - required
        - type: structure_wl_log
- `/software/wlconfig/structure_wl_logmonitor`
    - `/software/wlconfig/structure_wl_logmonitor/jobsPerCondorLog`
        - required
        - type: long
        - range: 1..
    - `/software/wlconfig/structure_wl_logmonitor/mainLoopDuration`
        - required
        - type: long
        - range: 1..
    - `/software/wlconfig/structure_wl_logmonitor/condorLogDir`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_logmonitor/condorRecycleDir`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_logmonitor/monitorInternalDir`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_logmonitor/idRepositoryName`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_logmonitor/abortedJobsTimeout`
        - required
        - type: long
        - range: 1..
    - `/software/wlconfig/structure_wl_logmonitor/externalLogFile`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_logmonitor/lockFile`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_logmonitor/log`
        - required
        - type: structure_wl_log
- `/software/wlconfig/structure_wl_networkserver`
    - `/software/wlconfig/structure_wl_networkserver/iiPort`
        - required
        - type: type_port
    - `/software/wlconfig/structure_wl_networkserver/iiTimeout`
        - required
        - type: long
        - range: 1..
    - `/software/wlconfig/structure_wl_networkserver/iiDN`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_networkserver/iiHost`
        - required
        - type: type_hostname
    - `/software/wlconfig/structure_wl_networkserver/grisPort`
        - required
        - type: type_port
    - `/software/wlconfig/structure_wl_networkserver/grisTimeout`
        - required
        - type: long
        - range: 1..
    - `/software/wlconfig/structure_wl_networkserver/grisDN`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_networkserver/backLogSize`
        - required
        - type: long
        - range: 0..
    - `/software/wlconfig/structure_wl_networkserver/listeningPort`
        - required
        - type: type_port
    - `/software/wlconfig/structure_wl_networkserver/masterThreads`
        - required
        - type: long
        - range: 0..
    - `/software/wlconfig/structure_wl_networkserver/dispatcherThreads`
        - required
        - type: long
        - range: 0..
    - `/software/wlconfig/structure_wl_networkserver/sandboxStagingPath`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_networkserver/quotaManagement`
        - required
        - type: boolean
    - `/software/wlconfig/structure_wl_networkserver/quotaSandboxSize`
        - required
        - type: long
        - range: 0..
    - `/software/wlconfig/structure_wl_networkserver/quotaAdjustment`
        - required
        - type: boolean
    - `/software/wlconfig/structure_wl_networkserver/quotaAdjustmentAmount`
        - required
        - type: long
        - range: 0..
    - `/software/wlconfig/structure_wl_networkserver/reservedDiskPercentage`
        - required
        - type: double
    - `/software/wlconfig/structure_wl_networkserver/log`
        - required
        - type: structure_wl_log
    - `/software/wlconfig/structure_wl_networkserver/DLICatalog`
        - optional
        - type: string
    - `/software/wlconfig/structure_wl_networkserver/RLSCatalog`
        - optional
        - type: string
- `/software/wlconfig/structure_wl_workloadmanager`
    - `/software/wlconfig/structure_wl_workloadmanager/pipeDepth`
        - required
        - type: long
        - range: 0..
    - `/software/wlconfig/structure_wl_workloadmanager/workerThreads`
        - required
        - type: long
        - range: 0..
    - `/software/wlconfig/structure_wl_workloadmanager/dispatcherType`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_workloadmanager/inputFile`
        - required
        - type: string
    - `/software/wlconfig/structure_wl_workloadmanager/maxRetryCount`
        - required
        - type: long
        - range: 1..
    - `/software/wlconfig/structure_wl_workloadmanager/log`
        - required
        - type: structure_wl_log
- `/software/wlconfig/wlconfig_component`
    - `/software/wlconfig/wlconfig_component/configFile`
        - required
        - type: string
    - `/software/wlconfig/wlconfig_component/user`
        - required
        - type: string
    - `/software/wlconfig/wlconfig_component/hostProxyFile`
        - required
        - type: string
    - `/software/wlconfig/wlconfig_component/grisCache`
        - required
        - type: long
        - range: 1..
    - `/software/wlconfig/wlconfig_component/useCachedResourceInfo`
        - required
        - type: boolean
    - `/software/wlconfig/wlconfig_component/jobController`
        - required
        - type: structure_wl_jobcontroller
    - `/software/wlconfig/wlconfig_component/logMonitor`
        - required
        - type: structure_wl_logmonitor
    - `/software/wlconfig/wlconfig_component/networkServer`
        - required
        - type: structure_wl_networkserver
    - `/software/wlconfig/wlconfig_component/workloadManager`
        - required
        - type: structure_wl_workloadmanager
