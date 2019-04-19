# oc-tests-nodejs
OpenShift NodeJS Tests

Deploy
******
Let's build the application with Openshift! Start it with "oc cluster up" then
    oc new-app https://github.com/romartin/oc-tests-nodejs.git --name=roger600-nodejs-test
Let's check that the service is available:
    oc get services
Finally, let's expose the route:
    oc expose service roger600-nodejs-test
Let's check the route:
    oc get routes

And finally:
    curl http://roger600-nodejs-test-roger600-nodejs-test.7e14.starter-us-west-2.openshiftapps.com


OC commands
************

DELETE - oc new-app labels everything that it creates, by default with app=<generated name>. You can use -l to customise the label(s) added to create resources:
    oc delete all -l app=roger600-nodejs-test

