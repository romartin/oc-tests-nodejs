# oc-tests-nodejs
OpenShift NodeJS Tests

Let's build the application with Openshift! Start it with "oc cluster up" then
    oc new-app https://github.com/romartin/oc-tests-nodejs.git --context-dir=roger600-nodejs-test --name=roger600-nodejs-test
Let's check that the service is available:
    oc get services
Finally, let's expose the route:
    oc expose service nodejs-basic
Let's check the route:
    oc get routes

And finally:
    curl http://nodejs-basic-myproject.192.168.1.66.xip.io