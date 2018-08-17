Modules
=======

A Drupal module is a collection of files containing some functionality and is written in PHP. All customizations, updates and patches need to be done within sites/all/.. directory. The modules and themes should not be updated or changed within the DKAN folder (profiles/dkan).::

   sites/
      all/
         libraries/ (your libraries)
         modules/ (your modules)
            contrib/ (modules from Drupal)
            custom/ (custom modules)
         themes/ (your themes)



		 
.. toctree::
   :maxdepth: 1

   Core modules <core>
   DKAN <dkan>
   Extensions <extensions>
   Custom <custom>   
