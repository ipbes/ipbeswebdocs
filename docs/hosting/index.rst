Web hosting
===========
The IPBES website is hosted on Pantheon_. The advantages of this are:
- Git workflow
- Daily backup
- Staging environments
- Support

The Pantheon workflow requires code to be committed to dev and pulled up to <test> and <live> environments. Database changes and pull down from <live> to <dev>

.. image:: images/pantheon_workflow.png
   :alt: Pantheon code and database flows.
  
.. _Pantheon: www.pantheon.io
