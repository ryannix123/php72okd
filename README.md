# php72okd
PHP 7.2 Imagestream for OpenShift 3.x series

This JSON file can be imported into the OKD 3.x series so PHP 7.2 is available to all users through the catalog. The JSON file points to Redhat's public container registry, so no Redhat login is required to obtain the latest PHP container.

Step 1.
ssh into your console as root.

Step 2.
From the server's CLI, use the OpenShift oc tool to login as the cluster admin. i.e., oc login

Step 3.
Run oc apply -f https://raw.githubusercontent.com/ryannix123/php72okd/master/php72.json -n openshift

Step 4.
Log back into the web console. Create a new project. The PHP image stream should say 7.2.