# Apigee X Shared Flow Bundle

This repository contains a Shared Flow Bundle for Apigee X.

## Overview

Shared Flows in Apigee allow you to encapsulate reusable policies and logic that can be invoked from multiple API proxies. This bundle is designed to be imported and used across your Apigee X proxies to promote consistency and reduce duplication.

## Features

- Centralized policy management
- Reusable logic across proxies
- Easy maintenance and updates

## Usage

1. **Import the Shared Flow Bundle:**

   - In the Apigee X console, navigate to **Develop > Shared Flows**.
   - Click **+ Shared Flow** and upload the bundle from this repository.

2. **Invoke from API Proxy:**
   - In your API proxy, add a `<FlowCallout>` policy referencing this shared flow.
   - Example:
     ```xml
     <FlowCallout name="Call-Shared-Flow">
       <SharedFlowBundle>YOUR_SHARED_FLOW_NAME</SharedFlowBundle>
     </FlowCallout>
     ```

## Structure

```
sharedflowbundle/
├── policies/
├── proxies/
├── resources/
├── sharedflow.xml
```

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements.

## License

This project is licensed under the MIT License.
