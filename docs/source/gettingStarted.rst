Getting Started
===============

.. _createAccount:

Creating a Developer Account
----------------------------

To use Monoly Fabric, create a developer account on `web portal <https://monoly.com>`_.
Developers can use their email address to create a developer account.

Login to Developer Account
^^^^^^^^^^^^^^^^^^^^^^^^^^

Once registered, developers can sign-in to developer portal using their registered email 
address and the chosen password.
Successful login will take the user to developers' home page.
In case the developer has forgotten the password, 
it can be easily reset using the registered email address during Sign-in stage.

Add Development Environment
^^^^^^^^^^^^^^^^^^^^^^^^^^^

Developer portal offers a sandbox development environment, 
in the cloud, running Monoly Fabrics' service nodes. 
It provides an opportunity for developers to develop, 
integrate and test their applications with actual fabric nodes without 
worrying about setting up the infrastructure for running such nodes.

While creating a developer account, 
one development environment gets created by default. 
If developers require more than one environment, 
they can create them via `developer portal <https://monoly.com>`_.

Application Key
---------------

An API key is a token that a client provides when making API calls. 
Developers use API Keys to access Monoly Fabric API. 
These represent the required credentials and also identify the application 
which is using the fabric API. API key ensure that only the authorized 
applications access the fabric nodes.

Developers can create and manage API keys from their developers portal. 
Each development or production environment requires a separate API key.

Managing API key
^^^^^^^^^^^^^^^^

You can manage the API key for accessing your development environment from developer portal. 
Against each development environment, you can create API key, 
rotate it or take other actions.

For production environment, 
API key can be managed from respective enterprise admin portal.

Creating an API key
^^^^^^^^^^^^^^^^^^^

To create an API key:

* Login in to developer portal using your credentials
* Go to respective development environment section for which you need to create API key
* Click *Generate API key* to create a new API key

.. warning::
    Monoly Fabric API returns 401 *Unauthorized* response for requests with missing or invalid API key.

Guidelines
^^^^^^^^^^

* API keys are supposed to be a secret that only the client and server know.
* Like basic authentication, API key-based authentication is only considered secure if used together with other security mechanisms such as HTTPS/SSL.
* Do not embed API keys directly in code. API keys that are embedded in code can be accidentally exposed to the public.
* Do not store API keys in files inside your application's source tree.
* Delete unneeded API keys to minimize exposure to attacks.
* Rotate your API keys periodically.
