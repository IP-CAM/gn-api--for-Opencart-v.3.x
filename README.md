# Gestãonet Integration Module for OpenCart-3.x - Version 3.1.2 (BETA) #

: warning: ** This module is only compatible with OpenCart versions higher than 3.0.2.0. If you have a lower version of Opencart, check the correct version of the module to be downloaded in the [Versions] (# versions) section **

** In case of doubts, you can check the [Documentation] (https://docs.gerencianet.com.br) of the API at Gerencianet and, needing more details or information, contact us, via our [Channels of Communication] (https://gerencianet.com.br/central-de-ajuda). **

## Pre-installation

: warning: This step should only be followed if you have the old version of the Gestãonet / Opencart module and Opencart 3.0.x.

1 - Uninstall the old Gestãonet module;

2 - Delete the following files on the server where Opencart is installed (only if you have version 0.x of the Opencart Gerencianet Module :):

- store / admin / controller / payment / Gerencianet.php
- store / admin / language / en-gb / payment / Gerencianet.php
- store / admin / view / template / payment / Gerencianet.tpl

- store / catalog / controller / payment / Gerencianet.php
- store / catalog / language / en-gb / payment / Gerencianet.php
- store / catalog / model / payment / Gerencianet.php
- store / catalog / view / theme / default / template / payment / Gerencianet.tpl
- store / catalog / view / theme / default / template / payment / Gerencianet_payment.tpl
- store / catalog / view / theme / default / template / payment / Gerencianet_success.tpl

: warning: No directories should be deleted, only the files mentioned above.

## Installation

### Automatic

1. Download the [automatic module] installer (auto /).
2. In the OpenCart store administration, access the `System> Settings` menu and click on the` Edit` button. In the ** FTP ** tab, fill in the FTP access information for your hosting. Pay special attention to the FTP Root field (FTP Directory), which is the full path to the root directory where your OpenCart is installed. Then click on the `Save` button.
3. Access the menu `Extensions> Extension Installer`, click on the button ** Upload **, select the file 'Gerencianet.ocmod.zip' (mentioned in the first instruction) and wait for the installation to complete automatic.

* If you have previously installed the Gestãonet module, OpenCart can inform you that some files will be overwritten. Do not worry, as the installation will not affect any files that are not from the Gestãonet module already in your store.

Attention: Due to the size of the module installation file, it may be necessary to change the `php_max_upload` parameter of` php.ini` to a minimum of 3mb.


### Manual

1. Download the [files of the latest version of the module] (manual /).
2. Unzip the downloaded files and upload the ** admin **, ** catalog ** and ** lib ** folders into the main OpenCart * directory.

* If you have previously installed the Gestãonet module, OpenCart can inform you that some files will be overwritten. Do not worry, as the installation will not affect any files that are not from the Gestãonet module already in your store.


## Settings

When accessing `Extensions> Extensions`, you must select the type of extension you want. Choose `Payments`. You will already see the Gestãonet module available in the list. Click `install` to install the module and then` edit` to start the configuration.

Three tabs will be available to configure the module:

* General Settings
* Credentials
* Purchase Status

### General Settings

In this tab, the following properties can be configured:
* Mode: Determines whether the module is in test mode. In test mode you can generate fictitious charges to test the flow.
* Payments allowed: Determines what types of payments will be accepted by the module
* Boleto expiration days: Determines how many days the boleto will expire after the generation date
* Boleto payment discount: You can provide discount to customers who pay through Boleto Bancário.
* Boleto Bancário instructions: You can define four lines with up to 90 characters of Boleto Bancário instructions. If the lines are not filled, the standard instructions on the boleto will be displayed
* Update OpenCart order status automatically: Determines whether the module can automatically update the status of an order according to the update notifications sent by Gestãonet
* Sending an automatic e-mail from your store to notify the customer: Notify the customer by an e-mail from your store when an automatic status update is performed. Regardless of the option, Gerencianet will send an email to the client informing about the charge.
* Status: Determines whether the Gestãonet payments module is Active or Inactive.
