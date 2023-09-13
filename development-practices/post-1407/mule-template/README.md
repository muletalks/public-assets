# MuleSoft Application Template

This repository contains a simple yet effective MuleSoft Application Template that you can use as a foundation for your integration projects. This template follows best practices for structuring your MuleSoft projects and includes essential components for building robust integrations.

## Features

- **Modular Design**: The template is structured to support easy addition or removal of components, ensuring flexibility for various project requirements.

- **Global Error Handling**: The template includes a simplified error handling configuration that catches the main HTTP related errors.

- **Configurability**: The template is easily configurable, allowing you to adapt it to different environments using properties files.

- **Consistent Naming Conventions**: Clear and consistent naming conventions for components, flows, and variables enhance readability and maintenance.

- **Encryption Setup using AES Algorithm**: Can be used to encrypt any sensitive information in the property files.

## Future Enhancements

We are continuously working to improve this MuleSoft Application Template to meet the evolving needs of integration projects. In the near future, we plan to enhance this template with the following components:

- **Logging Framework**: Our upcoming update will include a centralized logging framework that can be easily referenced in all flows, eliminating the need to duplicate logging settings throughout the project and ensuring consistent, efficient logging practices.

- **Error Handling Framework**: We will introduce an error handling framework that provides comprehensive error handling capabilities to enhance the reliability of your integrations.

Stay tuned for these enhancements, which will further empower you to build efficient and reliable MuleSoft integration solutions.

## How to Use

1. Clone this repository to your local environment.

2. Open the project in Anypoint Studio or your preferred MuleSoft development environment.

3. Customize the template to meet your project's specific requirements.

4. Deploy and test your MuleSoft application based on this template.

### Starting the App in Anypoint Studio

For starting the app in Anypoint Studio, the following parameters are required:

**Program Args**:
-Dmule.env=dev
-Dmule.key=XXXXXX

**VM Args**:
-Danypoint.platform.gatekeeper=disabled

## Contribution

If you have any improvements or additional features you'd like to suggest, please feel free to open an issue or create a pull request. Your contributions are welcome!
