# HubSpot-Project-POC
A poc project with new config + structure

## Structure overview

### Components
This project contains:
- An Auth component that defines an app
  - Including this component in your project will generate a private app in HubSpot
- Two CRM card components
  - These components both require auth, which is specified in the component config
- Two serverless function components
  - This component also requires auth, which is specified in the component config
- A CMS JS Rendering component
- A library component that enables the sharing of code across components
  - Currently being consumed by the "My POC project card 1" and "My POC project function" components via "deps" in the component config

### hscomponent.json config
Users create project components using the standardizes hscomponent.json configuration file. The supported fields in the config are...
- **type:** `(string)` The type of this component
- **label:** `(string)` The user-friendly label for this component
- **uid:** `(string)` The uid of this component
- **auth:** `(string)` The uid of the auth component that we want to link
- **deps:** `(array[string])` The uid's of the library components that this component depends on
- **data:** `(object)` Any component-specific config options
