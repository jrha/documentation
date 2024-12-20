
############################
NCM\::Component\::opennebula
############################


****
NAME
****


ncm-opennebula: Configuration module for OpenNebula


***********
DESCRIPTION
***********


ncm-opennebula provides support for OpenNebula configuration for:


- server: setup OpenNebula server and hosts



- AII: add VM management support with OpenNebula



server
======


Features that are implemented at this moment:


* oned service configuration



* Sunstone service configuration



* OneFlow service configuration



* Adding/removing VNETs



* Adding/removing datastores (only Ceph and shared datastores for the moment)



* Adding/removing hosts



* Adding/removing OpenNebula regular users



* Adding/removing OpenNebula groups



* Adding/removing OpenNebula virtual clusters



* Adding/removing OpenNebula VM groups and roles



* Assign OpenNebula resources to virtual clusters



* Assign OpenNebula users to primary groups



* Updates OpenNebula ``\*_auth`` files



* Updates VMM kvmrc config file



* Updates VNM OpenNebulaNetwork config file



* Updates KVM PCI passthrough filter config file



* Cloud resource labels (OpenNebula >= 5.x)



OpenNebula installation is 100% automated. Therefore:


* All the new OpenNebula templates created by the component will include a QUATTOR flag.



* The component only will modify/remove resources with the QUATTOR flag set, otherwise the resource is ignored.



* If the component finds any issue during host configuration then the node is set as disabled.



INITIAL CREATION
----------------



- The schema details are annotated in the schema file.



- Example pan files are included in the examples folder and also in the test folders.



To set up the initial cluster, some steps should be taken:


1. First install the required Ruby gems in your OpenNebula server (only for OpenNebula 5.10 or older). You can use OpenNebula installgems addon : `https://github.com/OpenNebula/addon-installgems <https://github.com/OpenNebula/addon-installgems>`_.



- 2. The OpenNebula server(s) should have passwordless ssh access as oneadmin user to all the host hosts of the cluster.  e.g. by distributing the public key(s) of the OpenNebula host over the cluster.



- 3. Start OpenNebula services: ``# for i in '' -econe -gate -novnc -occi -sunstone; do service opennebula$i stop; done``



- 4. Run the component a first time.



- 5. The new oneadmin password will be available from ``/var/lib/one/.one/one_auth`` file. The old auth files are stored with .quattor.backup extension.



- 6. It is also possible to change sunstone service password, just include 'serveradmin' user and passwd within opennebula/users tree. In that case the component also updates the ``sunstone_auth`` file.






*******
METHODS
*******


make_one
========


Sets ``OpenNebula`` ``RPC`` endpoint info to connect to ONE API.


process_template
================


Detect and process ONE templates.
It could return a ``CAF::TextRender`` instance or a plain text template for ONE ``RPC``.


create_or_update_something
==========================


Creates/updates ONE resources based on resource type.


remove_something
================


Removes ``OpenNebula`` resources.


update_something
================


Updates ``OpenNebula`` resource templates.


detect_used_resource
====================


Detects if the resource is already there and if QUATTOR flag is present.


- Returns undef: resource not used yet.



- Returns 1: resource already used without QUATTOR flag.



- Returns -1: resource already used with QUATTOR flag set




Configure
=========


Configure basic OpenNebula server resources.

