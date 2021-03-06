
Welcome to Data Science Project Template
----------------------------------------

This repo serves as a template to generate a project structure and boilerplate 
code for **Pyspark apps for Data Science**\ , targeting Bigdata environment.
In addition to generating boilerplate code, the template also includes artifacts & scripts 
required to build, package and deploy the app via CI/CD pipeline, in a single click!

Getting started
~~~~~~~~~~~~~~~


#. 
   Install the latest Cookiecutter package

   .. code-block::

      pip install -U cookiecutter --index-url https://pypi.org/simple

#. 
   Have the following information handy

.. list-table::
   :header-rows: 1

   * - Item
     - Description
     - Example
   * - Project Name
     - Project short name - used to name the project folder, build artifact, etc.
     - my-ml-project
   * - App ID
     - Acme Application inventory ID - used to identify SCM repo, XL Release (XLR) template, etc.
     - 6000000001
   * - Email
     - Individual or Team email id @acme.com - used in app notifications, SonarQube code scan, etc.
     - project_devops@acme.com
   * - Use case ID
     - Bigdata use case ID - used by deployment scripts to identify use case service ID
     - acmeml
   * - Use case path
     - Bigdata use case path - used to set the use case deployment area, working and warehouse area, log storage, etc.
     - /acme/cto/acmeml
   * - XLR Template alias*
     - Name of the XL Release (XLR) template setup through Development Tool Central
     - acmeml-silver
   * - XLR Subscription ID*
     - XLR subscription token setup for the above XLR Template
     - uuid


*\*\ Needed for pipeline as code deployments only* 

Generate your project
~~~~~~~~~~~~~~~~~~~~~

.. code-block::

   cookiecutter https://stash.acme.com/stash/scm/6000000001/cookiecutter.git

Project files are written into a folder named after *Project Name*\ , in the current directory.

Feedback & Contributions
~~~~~~~~~~~~~~~~~~~~~~~~


* For questions, comments or feedback, please write to: `CTO ML Devops <mailto:ctomldevops@acme.com>`_
* For code contributions, please submit a pull request.
