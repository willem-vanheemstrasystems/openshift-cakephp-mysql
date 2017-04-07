# openshift-cakephp-mysql
OpenShift, CakePHP and MySQL

# OpenShift Command Line Interface (CLI) Tools

See also https://console.preview.openshift.com/console/command-line

To install 'oc' on Mac, download the application from the location described in above URL, then place it in /opt/local/bin. You should now be able to run the following command:

```javascript
oc --help
```

To ***LOGIN*** with the command line tool, run the command:

NOTE: When logged in on the openshift website, opening the above URL will show you your token.

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

The oc login command automatically creates and manages CLI configuration files. All information gathered by the command is stored in a configuration file located in ```~/.kube/config```.

The current CLI configuration can be viewed using the following command:

```javascript
oc config view
```

It will also show all users tokens.

You can ***LOG OUT*** of CLI using the oc logout command:

```javascript
oc logout
```

To ***DELETE*** the deployment config (dc) 'cakephp-mysql-persistent'  and all of its deployments of the project 'totaljs-001' run the command:

```javascript
oc delete dc cakephp-mysql-persistent -n totaljs-001
```

You will be prompted with text similar to the below:

```javascript
deploymentconfig "cakephp-mysql-persistent" deleted
```

