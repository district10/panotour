CMD 历史：

```bash
C:\Users\tzx\Downloads\pano\panotour>cf login -u XXXXXXXXX@qq.com -o DigitalLifeGIS -s Pano
API endpoint: https://api.ng.bluemix.net

Password>
Authenticating...
OK

Targeted org DigitalLifeGIS

Targeted space Pano



API endpoint:   https://api.ng.bluemix.net (API version: 2.54.0)
User:           XXXXXXXXX@qq.com
Org:            DigitalLifeGIS
Space:          Pano

C:\Users\tzx\Downloads\pano\panotour>cf push panotour
Using manifest file C:\Users\tzx\Downloads\pano\panotour\manifest.yml

Updating app panotour in org DigitalLifeGIS / space Pano as XXXXXXXXX@qq.com...
OK

Using route panotour.mybluemix.net
Uploading panotour...
Uploading app files from: C:\Users\tzx\Downloads\pano\panotour
Uploading 945.1K, 32 files
Done uploading
OK
Binding service panotour-AdvancedMobileAccess to app panotour in org DigitalLifeGIS / space Pano as XXXXXXXXX@qq.com...
OK
Binding service panotour-imfpush to app panotour in org DigitalLifeGIS / space Pano as XXXXXXXXX@qq.com...
OK
Binding service panotour-cloudantNoSQLDB to app panotour in org DigitalLifeGIS / space Pano as XXXXXXXXX@qq.com...
OK

Stopping app panotour in org DigitalLifeGIS / space Pano as XXXXXXXXX@qq.com...
OK

Starting app panotour in org DigitalLifeGIS / space Pano as XXXXXXXXX@qq.com...
Downloading liberty-for-java...
Downloading sdk-for-nodejs...
Downloading swift_buildpack_v2_0_3-20161217-1748...
Downloading dotnet-core...
Downloading php_buildpack...
Downloaded sdk-for-nodejs
Downloading swift_buildpack...
Downloaded swift_buildpack_v2_0_3-20161217-1748
Downloaded liberty-for-java
Downloaded dotnet-core
Downloading ruby_buildpack...
Downloaded php_buildpack
Downloading nodejs_buildpack...
Downloaded noop-buildpack
Downloading go_buildpack...
Downloaded ruby_buildpack
Downloading python_buildpack...
Downloaded java_buildpack
Downloading xpages_buildpack...
Downloaded nodejs_buildpack
Downloading liberty-for-java_v3_6-20161209-1351...
Downloaded swift_buildpack
Downloading staticfile_buildpack...
Downloaded go_buildpack
Downloading binary_buildpack...
Downloaded python_buildpack
Downloaded staticfile_buildpack
Downloading liberty-for-java_v3_5-20161114-1152...
Downloaded xpages_buildpack
Downloading sdk-for-nodejs_v3_9-20161128-1327...
Downloaded liberty-for-java_v3_6-20161209-1351
Downloading dotnet-core_v1_0_6-20161205-0912...
Downloaded binary_buildpack
Downloaded dotnet-core_v1_0_6-20161205-0912
Downloaded sdk-for-nodejs_v3_9-20161128-1327
Creating container
Downloading noop-buildpack...
Downloaded liberty-for-java_v3_4_1-20161030-2241
Downloading liberty-for-java_v3_4_1-20161030-2241...
Successfully created container
Downloading app package...
Downloaded app package (1.9M)
Downloading build artifacts cache...
Downloaded build artifacts cache (21.3M)
Staging...
-----> IBM SDK for Node.js Buildpack v3.10-20170119-1146
       Based on Cloud Foundry Node.js Buildpack v1.5.24
-----> Creating runtime environment

       NPM_CONFIG_LOGLEVEL=error
       NPM_CONFIG_PRODUCTION=true
       NODE_MODULES_CACHE=true
-----> Installing binaries
       engines.node (package.json):  0.12.x
       engines.npm (package.json):   unspecified (use default)

       Resolving node version 0.12.x via 'node-version-resolver'
       Installing IBM SDK for Node.js (0.12.18) from cache
       Using default npm version: 2.15.11
-----> Restoring cache
       Loading 2 from cacheDirectories (default):
       - node_modules
-----> Checking and configuring service extensions before installing dependencies
       Installing node modules (package.json)
-----> Checking and configuring service extensions after installing dependencies
-----> Installing App Management
-----> Caching build
       Clearing previous node cache
       - node_modules
       Saving 2 cacheDirectories (default):
       - bower_components (nothing to cache)
-----> Build succeeded!
       ├── bms-mca-token-validation-strategy@2.0.9
       ├── compression@1.6.2
       ├── cors@2.8.1
       ├── loopback@2.38.0
       ├── loopback-boot@2.23.0
       ├── loopback-connector-mysql@2.4.1
       ├── loopback-datasource-juggler@2.54.0
       ├── passport@0.3.2
       └── serve-favicon@2.4.0

Exit status 0
Staging complete
Uploading droplet, build artifacts cache...
Uploading build artifacts cache...
Uploading droplet...
Uploaded build artifacts cache (21.4M)
Uploaded droplet (37.9M)
Uploading complete
Destroying container
Successfully destroyed container

1 of 1 instances running

App started


OK

App panotour was started using this command `./vendor/initial_startup.rb`

Showing health and status for app panotour in org DigitalLifeGIS / space Pano as XXXXXXXXX@qq.com...
OK

requested state: started
instances: 1/1
usage: 512M x 1 instances
urls: panotour.mybluemix.net
last uploaded: Mon Feb 27 03:41:43 UTC 2017
stack: cflinuxfs2
buildpack: SDK for Node.js(TM) (ibm-node.js-0.12.18, buildpack-v3.10-20170119-1146)

     state     since                    cpu    memory           disk           details
#0   running   2017-02-27 11:43:37 AM   0.2%   261.8M of 512M   209.5M of 1G
```
