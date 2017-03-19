============================
OpenStack-Ansible MoltenIron
============================

Ansible role to deploy MoltenIron.

To clone or view the source code for this repository, visit the role repository
for `os_molteniron <https://github.com/openstack/openstack-ansible-os_molteniron>`_.

Default variables
~~~~~~~~~~~~~~~~~

.. literalinclude:: ../../defaults/main.yml
   :language: yaml
   :start-after: under the License.

Required variables
~~~~~~~~~~~~~~~~~~

To install molteniron nodes, please add the following set of information:
There can be more than one bare metal node.

  molteniron_baremetal_nodes:
    - name: test1
      ipmi_ip: 10.1.2.1
      ipmi_user: user
      ipmi_password: password
      allocation_pool: 10.1.2.3,10.1.2.4
      port_hwaddr: de:ad:be:ef:00:01
      cpu_arch: ppc64el
      cpus: 8
      ram_mb: 2048
      disk_gb: 32

Example playbook
~~~~~~~~~~~~~~~~

.. literalinclude:: ../../examples/playbook.yml
   :language: yaml
