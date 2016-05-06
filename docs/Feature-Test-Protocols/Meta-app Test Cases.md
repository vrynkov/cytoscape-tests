# Test Cases for Meta-apps

**1. Build meta-app from archetype**
 * Run mvn archetype:generate with Meta-App archetype installed
 * Provide a name and a package/groupID
 * Edit the project pom.xml and add dependencies in the Cytoscape-App-Dependencies heading on several apps. Include apps that have their own dependencies
 * Build the project
 * Submit resulting JAR to the App Store
 * Add tag to designate meta-app as theme

**2. Build another meta-app from archetype**
 * Run mvn archetype:generate with Meta-App archetype installed
 * Provide a name and a package/groupID
 * Edit the project pom.xml and add dependencies in the Cytoscape-App-Dependencies heading on several apps. Include the first meta-app created above as well as some other app. 
 * Build the project
 * Submit resulting JAR to the App Store
 * Add tag to designate meta-app as theme

**3. Install meta-app from App Manager**
 * Start Cytoscape w/meta-app in App Store (test server set up with App Manager)
 * Open App Manager
 * Install meta-app
 * Verify that all component apps and dependencies are installed
 * Restart Cytoscape and repeat for other meta-app

**4. Update meta-app from App Manager**
* Start Cytoscape w/meta-app update in App Store (test server set up with App Manager)
* Open App Manager
* Install update in “Check for Updates” tab
* Verify that added apps are installed
* Restart Cytoscape and repeat for other meta-app

**5. Update meta-app components from App Manager**
* Start Cytoscape w/new updates to apps installed by meta-apps
* Open App Manager
* Install updates in “Check for Updates” tab
* Verify that updates have installed properly
* Restart Cytoscape and repeat for other meta-app

**6. Uninstall meta-app from App Manager**
* Start Cytoscape with installed meta app
* Open App Manager
* Uninstall meta-app from “Currently Installed” tab
* Verify that meta-app has been uninstalled, but not component apps
* Restart Cytoscape and repeat for other meta-app

**7. Install meta-app from App Store**
 * Start Cytoscape w/meta-app in App Store (test server set up with App Manager)
 * Open App Store in web browser and open app page
 * Install meta-app
 * Verify that all component apps and dependencies are installed
 * Restart Cytoscape and repeat for other meta-app

**8. Update meta-app from App Store**
 * Start Cytoscape w/meta-app update in App Store (test server set up with App Manager)
 * Open App Store in web browser and open app page
 * Install update
 * Verify that added apps are installed
 * Restart Cytoscape and repeat for other meta-app

**9. Update meta-app components from App Store**
 * Start Cytoscape w/new updates to apps installed by meta-apps
 * Open App Store in web browser and open page of an updated app
 * Install update
 * Repeat least two steps for each update
 * Verify that updates have installed properly
 * Restart Cytoscape and repeat for other meta-app

**10. Install meta-app from file**
 * Start Cytoscape 
 * Open App Manager
 * Install meta-app
 * Verify that all component apps and dependencies are installed
 * Restart Cytoscape and repeat for other meta-app
 * Repeat both with no internet connection (should give error resolving dependencies/abort install)
 * Repeat installing all at once with no internet connection (should work)

**11. Update meta-app from file**
 * Start Cytoscape 
 * Open App Manager
 * Install meta-app update from file
 * Verify that added apps are installed
 * Restart Cytoscape and repeat for other meta-app
 * Repeat both with no internet connection (should give error resolving dependencies/abort install)
 * Repeat installing all at once with no internet connection (should work)


**12. Update meta-app components from file**
 * Start Cytoscape 
 * Open App Manager
 * Install meta-app update from file
 * Verify that updates have installed properly
 * Restart Cytoscape and repeat for other meta-app
 * Repeat both with no internet connection (should work if all dependencies are present - otherwise it should abort with error)
