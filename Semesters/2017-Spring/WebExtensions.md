# WebExtensions

## Browser Extensions:
  - Add features (easier)
  - Customize and protect your experience
  - Caveats
    - Callbacks
    - Promises
    - Polyfill
    - Not all browsers support all API's (look at a compatibility chart for more info)

## Parts to a Web Extension:

- Manifest
  - Metadata, Permissions, and other files
- Content Script
  - Loaded onto page (or specific pages), Manipulates the DOM, don't have access to all of API (due to security, so they use "messages")
- Background Scripts
  - Persistent, access to full API, no DOM access
- Popup/Menu
  - Browser icon, Side bars, Rick click menu, Dev tools, etc.
- Extension Page
  - Dedicated page only for extension, non-persistent, full API access, Not in manifest.json
- Web Resources
  - All resources needed for API are here: Images, Music, etc.

## Web Extensions are Simple:

- Theme
  - Header Image, UI colors
  - Events for new theme
- Tabs
    - Information about tabs: url, Favicon
    - Execute scripts, Reload or close
- Storage
  - Save content, Asynchronous access, Sync across browsers
- Runtime
  - Part of the message passing system
  - Can talk to Native Applications
- i18n
  - Internationalization
  - Switch languages (or replace strings)
- Other API:
  - BrowsingData
    - access to cookies, cache, etc.
  - DNS
    - Find out which DNS server your talking to, do stuff with it
  - Privacy
    - Access to privacy setting for browser, Ex: change cookie policy of browser
  - Commands
    - Access to Hotkeys, add hotkeys etc.
  - WebNavigation
    - How you move through sites (abstracted from HTTP)
  - WebRequests
    - Access to look at and modify HTTP Requests
  - Even more exist!

## Extensions are Powerful

### Resources:
- Mozilla Developer Network
  - START HERE
- Chrome Documentation
- Edge Documentation
