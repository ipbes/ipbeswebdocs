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
		 
Menu
----
Used for navigation

Content types
-------------
A Content Type is a set of fields for a particular type of data.  Content types contain a field for the node title and second field for the body into which the node content is placed. The title and body fields display information to the user.  Additional fields for a node store url and redirect settings.

Taxonomy vocabularies
---------------------
Reference lists

Modules
-------
A Drupal module is a collection of files containing some functionality and is written in PHP. 

Themes
------
Themes control the design, look and feel of the website using HTML, CSS, JavaScript, and other front-end assets in order to implement a design for their site. Themes are used to change the HTML markup of anything in Drupal; Add CSS styles to change the layout, color, or typography on one or more pages; and Use JavaScript to enhance the user experience


.. toctree::
   :maxdepth: 1
   
   Menu <menu>
   Content Types <content-types>
   Taxonomy vocabularies <taxonomy-vocabularies>
   modules/index
   Theme <theme>

.. _ipbes website: https://www.ipbes.net
.. _policy support: https://www.ipbes.net/policy-support
