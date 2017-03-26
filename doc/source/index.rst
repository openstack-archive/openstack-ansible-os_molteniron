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

.. literalinclude:: ../../examples/required_variables.yml
   :language: yaml

Example playbook
~~~~~~~~~~~~~~~~

.. literalinclude:: ../../examples/playbook.yml
   :language: yaml
