# openshift-cakephp-mysql
OpenShift, CakePHP and MySQL

# OpenShift Command Line Tools

See also https://console.preview.openshift.com/console/command-line

To install 'oc' on Mac, download the application from the location described in above URL, then place it in /opt/local/bin. You should now be able to run the following command:

```javascript
oc --help
```

To ***DELETE*** the deployment config (dc) 'cakephp-mysql-persistent'  and all of its deployments of the project 'totaljs-001' run the command:

```javascript
oc delete dc cakephp-mysql-persistent -n totaljs-001
```

