Review, update and uninstall modules using drush
================================================
It is better to use drush instead of git because drush will check to see dependencies of the module before uninstalling and prompt you to uninstall/check dependent modules.
 
Requirements
------------
- A mac computer with terminal
- drush http://docs.drush.org/en/master/install/
- drush aliases from your user dashboard: https://pantheon.io/blog/drush-aliases-available
- Machine name of module which is the name of the module folder in sites/all/modules/contrib
 
Preparation
-----------
- Back up any view or page that is using the module
- Make sure that no view or page is using the module
- Disable module on live
- Clone live environment to dev
- Make sure that the module is contained in sites/all/modules/contrib and that you are not uninstalling a module that comes with the site distribution package
- Do a manual backup of site

Steps for updating
------------------
- Log into Pantheon and go to the dev environment
- Switch development mode from git to SFTP
- Go to terminal on Mac and change directory to the project folder e.g. cd ipbesnew
- Type in the following command: drush @pantheon.ipbesnew.dev up [machine name of module]
- Confirm that you wish to disable the module
- Go back to the pantheon dashboard and add a commit message
- Switch site back to git mode

Steps for uninstalling
------------------
- Log into Pantheon and go to the dev environment
- Switch development mode from git to SFTP
- Go to terminal on Mac and change directory to the project folder e.g. cd ipbesnew
- Type in the following command: drush @pantheon.ipbesnew.dev pmu [machine name of module]
- Confirm that you wish to disable the module
- Go back to the pantheon dashboard and add a commit message
- Switch site back to git mode
