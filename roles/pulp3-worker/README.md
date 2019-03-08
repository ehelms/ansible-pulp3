pulp-workers
=============

Install, configure, and set the state of pulp workers.

Configurable Variables:
-----------------------

* `pulp_worker_count`: Specify how many workers are desired. Defaults to
  2 workers which are started and enabled by systemd.

Shared variables:
-----------------

* `ansible_python_interpreter`: **Required**. Path to the Python interpreter.

This role **is tightly coupled** to the required `pulp3-redis` and `pulp3` role, and inherits
some of its variables.

* `pulp_user`
* `pulp_install_dir`

Dependencies:
-------------

* `pulp3-redis`
* `pulp3`
