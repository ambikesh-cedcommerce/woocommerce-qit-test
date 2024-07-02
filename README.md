
# How to get started with WooCommerce Qit Test

Introduction:
Before delving into the specifics of WooCommerce Qit Test, you might be wondering what it means and why it's essential for your plugin/theme. I'll elaborate on the significance of WooCommerce Qit Test and why it is crucial for your extension's success.

#### Understanding WooCommerce Qit Test:
The WooCommerce Qit Test is implemented to ensure that all extensions available in the Woo Marketplace meet the highest quality standards. This involves a series of automated tests that thoroughly assess the functionality, security, and compatibility of your plugin/theme.


## Types of Tests: : 

#### 1) End-to-End (e2e) Test : 
- The end-to-end (e2e) test creates a temporary WordPress installation with WooCommerce and the extension under test installed, and uses a browser that is scripted to perform certain automated tasks, such as completing the WooCommerce onboarding wizard, creating a product, making a purchase as a customer, verifying the order details as an admin, tweaking tax settings, etc.
#### 2) Activation Test :
- The Activation test type activates your extension against a freshly created shop and captures any PHP errors or warnings that may occur on activation.
#### 3) Security Test :
- This test runs an experimental security scanner against a given extension.
#### 4) PHPStan Test : 
- The PHPStan test type runs level 0 PHPStan checks against your extension. More details on what the rule levels cover can be found in the official PHPStan documentation: Rule Levels. 
 #### 5) API Test :
 -  API Testing is a crucial part of ensuring the smooth functioning of an application. With API testing, we execute a set of operations using the WooCommerce REST API and verify that the API responds in an expected, consistent, way.
#### 6) PHPCompatibility Test : 
 - The PHPCompatibility test is a tool that helps developers assess the compatibility of their extension with different PHP versions. It checks the codebase of a plugin against a set of coding standards and best practices to ensure that it can run on a wide range of PHP versions, ensuring better compatibility and security.

### 7) Malware Test: 
 - Our malware scanner is designed to detect and identify potentially malicious or suspicious PHP code in web applications and files. It is primarily used for identifying PHP-based malware, backdoors, and other security threats that may have been injected into PHP files.


## Install WooCommerce Qit

To install WooCommerce qit on your local computer follow the commands below

```bash
  composer require woocommerce/qit-cli --dev
```

To execute and authenticate with your Woo.com Partner Developer account.

```bash
 ./vendor/bin/qit
 ```


 ## Install Qit

[To install qit on your local computer](https://woocommerce.github.io/qit-documentation/#/cli/getting-started?id=installing-qit)


## Run Locally
 End-to-End Tests
 ```bash
./vendor/bin/qit run:e2e my-plugin-slug --zip=my-plugin-slug
```
 Activation Tests
```bash
./vendor/bin/qit run:activation my-plugin-slug --zip=my-plugin-slug
```
 Security Tests
```bash
./vendor/bin/qit run:security my-plugin-slug --zip=my-plugin-slug
```
 PHP Stan Tests
```bash
./vendor/bin/qit run:phpstan my-plugin-slug --zip=my-plugin-slug
```
 API Tests
```bash
./vendor/bin/qit run:api my-plugin-slug --zip=my-plugin-slug
```
 PHP Compatibility Tests
```bash
./vendor/bin/qit run:phpcompatibility my-plugin-slug --zip=my-plugin-slug
```
 Malware Tests
```bash
./vendor/bin/qit run:malware my-plugin-slug --zip=my-plugin-slug
```

### Testing a published extension

```bash
 qit run:e2e my-extension --zip=my-plugin-slug
```

## Documentation

[Documentation]([https://woocommerce.github.io/qit-documentation/#/](https://qit.woo.com/docs/))

