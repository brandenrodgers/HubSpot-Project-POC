# HubSpot-Project-POC
A poc project with new config + structure

## Structure overview

#### Components
This project contains:
- An Auth component that defines an app
- Two CRM card components
- Two serverless function components
- A CMS JS Rendering component
- A library component that enables the sharing of code across components
  - Currently being consumed by the "My POC project card 1" and "My POC project function" components

#### hscomponent.js component config
- **type:** `(string)` The type of this component
- **label:** `(string)` The user-friendly label for this component
- **uid:** `(string)` The uid of this component
- **auth:** `(string)` The uid of the auth component that we want to link
- **deps:** `(array[string])` The uid's of the library components that this component depends on
- **data:** `(object)` Any component-specific config options
