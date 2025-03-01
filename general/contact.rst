.. _contact:

#######
Contact
#######

GitHub
******
Our preference is to use GitHub for communication. The reason for that is that
it is an open source project, so there should be no real reason to hide
discussions from other people. GitHub also makes it possible for anyone to chime
in into discussion etc. So besides sending patches as pull requests on GitHub we
also encourage people to use the "issues_" to report bugs, give suggestions, ask
questions etc.

Please try to use the "issues" in the relevant git. I.e., if you want to discuss
something related to optee_client, then use "issues" at :ref:`optee_client` and
so on. If you have a general question etc about OP-TEE that doesn't really
belong to a specific git, then please use `issues at optee_os`_ in that case.

Email
*****
You can reach the :ref:`core_team` by sending an email to
``op-tee[at]lists.trustedfirmware.org``. However note that it's a public
mailinglist and **not** just TrustedFirmware engineers behind that email
address.

For pure Linux kernel patches, please use the appropriate Linux kernel
mailinglist, basically run the ``get_maintainer.pl`` script in the Linux kernel
tree to figure out where to send your patches.

.. code-block:: bash

    $ cd <linux-kernel>
    $ ./scripts/get_maintainer.pl drivers/tee/


IRC
***
Some of the OP-TEE developers can be reached at Freenode (``chat.freenode.net``)
at channel ``#linaro-security``. Having that said, the activity there is a bit
limited, so it is probably **not** the best place to discuss OP-TEE.

.. _vulnerability_reporting:

Vulnerability reporting
***********************
The OP-TEE project as part of the TrustedFirmware.org organization is using the
security incident process as described at the `TrustedFirmware.org security incident`_
page. To report an issue, please follow the process as specified here. The email
address to use can be found at the `Mailing Aliases`_ page.

Note that OP-TEE is a reference implementation for developers and device
manufacturers and by being a reference implementation it is not always running a
secure device configuration by default (see :ref:`platform_ports` for more
information). Therefore we ask people to think twice whether the security
incident report should go to:

 a) The OP-TEE project? Is it an issue in the generic code?
 b) The chipmaker? Does it only affect a certain platform? Is it a configuration described only under NDA?
 c) The ones making the end product? Is the issue only present on a certain device?

The OP-TEE team are in some cases are working directly with chipmakers. But it's
not uncommon that products are made using OP-TEE that the OP-TEE project is
unaware of. In those cases we would recommend sending the security issue report
to the company making the end product and that they in turn and if needed reach
out to the OP-TEE project and/or the chipmaker.

.. _core_team:

Core Team
*********
The core team consists of engineers from TrustedFirmware.org. Related, see the
`core team`_ at GitHub.

.. _core team: https://github.com/orgs/OP-TEE/teams/linaro/members
.. _issues: https://help.github.com/articles/about-issues/
.. _issues at optee_os: https://github.com/OP-TEE/optee_os/issues
.. _Mailing Aliases: https://developer.trustedfirmware.org/w/collaboration/security_center/mailing_aliases
.. _TrustedFirmware.org security incident: https://developer.trustedfirmware.org/w/collaboration/security_center
