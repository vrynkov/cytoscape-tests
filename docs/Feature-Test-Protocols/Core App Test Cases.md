# Test Cases for Core Apps
**1. Initial install of core apps (empty CytoscapeConfiguration)**
 * Start Cytoscape with empty CytoscapeConfiguration directory
 * Open App Manager
 * Verify that all core apps installed properly
 * Restart Cytoscape and verify again

**2. Update core app**
 * Start Cytoscape with available core app updates
 * Open App Manager and check for updates
 * Install available updates
 * Verify that updates installed correctly
 * Restart Cytoscape and verify again

**3. Uninstall core app update**
 * Start Cytoscape with available core app updates
 * Open App Manager and check for updates
 * Uninstall updates
 * Verify that updates uninstalled correctly and old versions restored

**4. Install bundle app by App Manager**
 * Start Cytoscape with available core app updates
 * Open App Manager
 * Install an app
 * Verify that it installed OK
 * Restart Cytoscape and verify again

**5. Update bundle app**
 * Start Cytoscape with available core app updates
 * Open App Manager and check for updates
 * Install available updates
 * Verify that updates installed correctly
 * Restart Cytoscape and verify again

**6. Uninstall bundle app**
 * Start Cytoscape with available core app updates
 * Open App Manager
 * Install an app
 * Verify that it installed OK
 * Restart Cytoscape and verify again

**7. Install bundle app by copy**
 * Start Cytoscape with available core app updates
 * Copy an app to the installed directory
 * Verify that it installed OK
 * Restart Cytoscape and verify again

**. Uninstall bundle app by delete**
 * Start Cytoscape with available core app updates
 * Copy an app to the installed directory
 * Verify that it installed OK
 * Restart Cytoscape and verify again

**9. Install bundle app via App Store**
 * Start Cytoscape 
 * Open App Store in browser
 * Install an app
 * Verify that the app installed correctly
 * Restart Cytoscape and verify again

**10. Disable App in App Manager**
 * Start Cytoscape
 * Open App Manager
 * Disable an app
 * Verify that the app disabled correctly
 * Restart Cytoscape and verify again

**11. Enable App in App Manager**
 * Start Cytoscape
 * Open App Manager
 * Enable an app
 * Verify that the app re-enabled correctly
 * Restart Cytoscape and verify again

**12. Install simple app**
 * Start Cytoscape
 * Open App Manager
 * Install a simple app
 * Verify that it installed OK
 * Restart Cytoscape and verify again

**13. Update simple app**
 * Start Cytoscape with available simple app updates
 * Open App Manager and check for updates
 * Install available updates
 * Verify that updates installed correctly
 * Restart Cytoscape and verify again

**14. Disable simple app**
 * Start Cytoscape
 * Open App Manager
 * Disable simple app
 * Verify that the simple app disabled correctly
 * Restart Cytoscape and verify again

**15. Enable Simple app**
 * Start Cytoscape
 * Open App Manager
 * Enable simple app
 * Verify that the app re-enabled correctly
 * Restart Cytoscape and verify again

**16. Uninstall Simple app**
 * Start Cytoscape
 * Open App Manager
 * Uninstall simple app
 * Verify that the app uninstalled correctly
 * Restart Cytoscape and verify again

**17. Install multiple versions**
 * Start Cytoscape
 * Install an older version of an app using Install from File
 * Install a newer version of an app using Install from File
 * Verify that only newer version is installed
 * Reinstall the older version using Install from File
 * Verify that only older version is installed
 * Restart Cytoscape and verify again

**18. Copy older and then newer version**
 * Start Cytoscape
 * Copy an older version of an app to the installed directory
 * Copy a newer version of the same app to the installed directory
 * Verify that only newer version is installed
 * Restart Cytoscape and verify again

**19. Copy newer and then older version**
 * Start Cytoscape
 * Copy an newer version of an app to the installed directory
 * Copy a older version of the same app to the installed directory
 * Verify that newer version is still installed (and not older)
 * Restart Cytoscape and verify again

**20. Upgrade app from App Store**
 * Start Cytoscape
 * Go to App Store and bring up page for already-installed app with updates available
 * Click “Upgrade”
 * Verify that it installed OK
 * Restart Cytoscape and verify again

**21. Rebuild based on symbolic link**
 * Start Cytoscape with app symbolicly-linked from target directory
 * Verify app installed correctly
 * Rebuild app with no changes
 * Verify app still installed
 * Rebuild app with version number change
 * Verify app updated correctly.

**22. Incompatible bundle app**
 * Start Cytoscape
 * Install bundle app with incompatible update available (i.e. one that depends on 3.4 - edit manifest to achieve this)
 * Try to install update via Update Manager
 * Try to install update with Install from File
 * Try to copy update (app should not load in any of the previous cases)
 * Restart Cytoscape and verify that old compatible app loaded/new incompatible app not loaded

**23. Incompatible simple app**
 * Start Cytoscape
 * Install simple app with incompatible update available (i.e. one that depends on 3.4 - edit manifest to achieve this)
 * Try to install update via Update Manager
 * Try to install update with Install from File
 * Try to copy update (app should not load in any of the previous cases)
 * Restart Cytoscape and verify that old compatible app loaded/new incompatible app not loaded
