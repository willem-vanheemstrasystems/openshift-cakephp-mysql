# openshift-cakephp-mysql
OpenShift, CakePHP and MySQL

# OpenShift Command Line Tools

See also https://console.preview.openshift.com/console/command-line

To install 'oc' on Mac, download the application from the location described in above URL, then place it in /opt/local/bin. You should now be able to run the following command:

```javascript
oc --help
```

To ***LOGIN*** with the command line tool, run the command:

```javascript
oc login https://api.preview.openshift.com --token=<TOKEN PROVIDED, KEEP IT SECRET>
```

You will be prompted with a text similar to the below:

```javascript
Logged into "https://api.preview.openshift.com:443" as "willem-vanheemstrasystems" using the token provided.

You have one project on this server: "totaljs-001"

Using project "totaljs-001".
Welcome! See 'oc help' to get started.
```

To ***DELETE*** the deployment config (dc) 'cakephp-mysql-persistent'  and all of its deployments of the project 'totaljs-001' run the command:

```javascript
oc delete dc cakephp-mysql-persistent -n totaljs-001
```

You will be prompted with text similar to the below:

```javascript
deploymentconfig "cakephp-mysql-persistent" deleted
```

