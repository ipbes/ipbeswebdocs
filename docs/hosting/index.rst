Web and domain name hosting
===========================

Web hosting
-----------
The IPBES website is hosted on Pantheon_. The advantages of this are:

- Git workflow
- Daily backup
- Staging environments
- Support

The Pantheon workflow requires code to be committed to dev and pulled up to <test> and <live> environments. Database changes and pull down from <live> to <dev>

.. image:: ../images/hosting_pantheon_workflow.png
   :alt: Pantheon code and database flows.

Domain name hosting
-------------------
The domain name services (DNS) are hosted by gandi.net


.. toctree::
   :maxdepth: 1
   
.. _Pantheon: www.pantheon.io
