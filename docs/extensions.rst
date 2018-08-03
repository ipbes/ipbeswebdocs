Extending and Customizing the website
===============================
The IPBES website is based on DKAN, a `Drupal
Distribution <https://drupal.org/documentation/build/distributions>`_. Additional modules have been
added to extend functionality. Modules are added from contributed modules available from the Drupal Community `contrib  modules <https://www.drupal.org/project/project_module>`_ from the Drupal community. However, as 

DKAN consists of of a distribution profile which manages the initial
installation, 3rd party libraries and drupal modules, and DKAN specific
modules.

Below is a simplified version of where the DKAN code sits within the fully
packaged version::

   profiles/
       dkan/
         libraries/ (3rd party libraries)
         modules/
            dkan/ (dkan modules)
            contrib/ (3rd party module dependencies)
         themes/ (dkan themes)
   sites/
      all/
         libraries/ (your libraries)
         modules/ (your modules)
         themes/ (your themes)

After installing DKAN additional functionality should be added to the "sites"
directory.

In the future, this section will feature more detailed information on developing
custom extentions to DKAN. For now, read additional information about:
