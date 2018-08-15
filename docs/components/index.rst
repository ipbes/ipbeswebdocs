Major components
================

The IPBES website is based on DKAN, a `Drupal
Distribution <https://drupal.org/documentation/build/distributions>`_. Additional modules have been added to extend functionality. Modules are added from contributed modules available from the Drupal Community `contrib  modules <https://www.drupal.org/project/project_module>`_ from the Drupal community. 

DKAN consists of of a distribution profile which manages the initial installation, 3rd party libraries and drupal modules, and DKAN specific modules. Below is a simplified version of where the DKAN code sits within the code::

   profiles/
       dkan/
         libraries/ (3rd party libraries)
         modules/
            dkan/ (dkan modules)
            contrib/ (3rd party module dependencies)
         themes/ (dkan themes)

The modules and themes should not be updated or changed within the DKAN folder. All customizations, updates and patches need to be done within sites/all/.. directory::

   sites/
      all/
         libraries/ (your libraries)
         modules/ (your modules)
            contrib/ (modules from Drupal)
            custom/ (custom modules)
         themes/ (your themes)
		 
- Menu
- Content types
- Taxonomy vocabularies
- Modules
- Themes


.. toctree::
   :maxdepth: 1
   
   Menu <menu>
   Content Types <content-types>
   Taxonomy vocabularies <taxonomy-vocabularies>
   modules/index
   Theme <theme>

.. _ipbes website: https://www.ipbes.net
.. _policy support: https://www.ipbes.net/policy-support
