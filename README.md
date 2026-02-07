haxwithaxe.ardopcf
================

Install ardopcf.

Requirements
------------

* A debian install.
* This must be run as a user with read and write access to `ardopcf_src_dir` and the install target for `make install` in the `ardopcf` source (`/usr/local/bin`).
* Installs ``build-essentials``, ``libasound-dev``, and ``git`` if they aren't present already.

Role Variables
--------------

- `ardopcf_git_url` - The URL of the `ardopcf` git repository. Defaults to ``https://github.com/pflarue/ardop.git``.
- `ardopcf_git_version` - The git commit/ref/tag to checkout for building. Defaults to ``develop``.
- `ardopcf_installed_executable` - The path of the installed `ardopcf` executable. Defaults to ``/usr/local/bin/ardopcf``.
- `ardopcf_src_dir` - The path where the `ardopcf` source code will be stashed. Defaults to ``/usr/local/src/ardopcf``.


Dependencies
------------

None.


Example Playbook
----------------

To install with all default values:

    - hosts: ham_computers
      roles:
         - role: haxwithaxe.ardop


License
-------

GPL-3.0-only


Author Information
------------------

Created by [haxwithaxe W3AXE](https://github.com/haxwithaxe).
