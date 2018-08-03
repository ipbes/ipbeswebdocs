Major components
================

Menu
----
You have two options for formatting your documentation:

Main menu
~~~~~~~~~
Main menu

User menu
~~~~~~~~~~
User menu

Policy support menu
~~~~~~~~~~~~~~~~~~~

You can use Markdown and reStructuredText in the same Sphinx project.
We support this natively on Read the Docs, and you can do it locally.

.. note:: The policy support catalogue structure is maintained by WCMC and OPPLA
          and changes to the menu structure needs to be done in consultation with them.

Content types
-------------
List of content types and what they do

taxonomy vocabularies
---------------------

To import a repository, visit your dashboard and click Import.

Manually Import Your Docs
~~~~~~~~~~~~~~~~~~~~~~~~~

If you do not have a connected account, you will need select **Import Manually**
and enter the information for your repository yourself. You will also need to
manually configure the webhook for your repository as well. When importing your
project, you will be asked for the repository URL, along with some other
information for you new project. The URL is normally the URL or path name you'd
use to checkout, clone, or branch your repository. Some examples:

* Git: ``http://github.com/ericholscher/django-kong.git``
* Mercurial: ``https://bitbucket.org/ianb/pip``
* Subversion: ``http://varnish-cache.org/svn/trunk``
* Bazaar: ``lp:pasta``

Add an optional homepage URL and some tags, and then click **Next**.

Once your project is created, you'll need to manually configure the repository
webhook if you would like to have new changesets to trigger builds for your
project on Read the Docs. Go to your project's **Integrations** page to
configure a new webhook, or see :ref:`our steps for webhook creation <webhooks:Webhook Creation>`
for more information on this process.

Within a few seconds your code will automatically be fetched from your public repository,
and the documentation will be built.
Check out our :doc:`builds` page to learn more about how we build your docs,
and to troubleshoot any issues that arise.

Read the Docs will host multiple versions of your code. You can read more about
how to use this well on our :doc:`versions` page.


If you have any more trouble, don't hesitate to reach out to us. The :doc:`support` page has more information on getting in touch.

.. _ipbes website: https://www.ipbes.net
.. _policy support: https://www.ipbes.net/policy-support
