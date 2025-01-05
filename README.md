# Firefox-Ash-Dark

##  Setting up userChrome.css & userContent.css on firefox

  1. Go to about:config

  2. Set the pref toolkit => legacyUserProfileCustomizations.stylesheets to true (default is false)

  3. (Optional Step - To enable dark theme as default) Create new pref as => ui.systemUsesDarkTheme = 1

  4. Open about:support

  5. Click on "Profile Folder" -> "Open Folder"

  6. Create a sub-folder named "chrome" if it doesn't already exist

  7. Open the "chrome" folder and create a file named "userChrome.css" & "userContent.css"

  8. Add some rules

  9. Restart Firefox


## Optional about:config tweaks

/* Tab min width (suggestion: 125) */
  browser.tabs.tabMinWidth

/* Disable Pocket */
  extensions.pocket.enabled = false

/* In order to enable extensions to change styles of blocked domains change the following two configs*/ 
  1. Add the pref to about:config => privacy.resistFingerprinting.block_mozAddonManager = true

  2. Remove the domain name from this pref => extensions.webextensions.restrictedDomains

/* Disable Accessibility - Helps reduce memory usage? */
  accessibility.force_disabled = 1

/* Restore download prompt in Firefox 98 */
  browser.download.improvements_to_download_panel = false.