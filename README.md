# NetXsecure WPA3 Enterprise Enhancements

## Overview

The NetXsecure WPA3 code from Azure RTOS is enhanced to support the following

- Add TLS 1.3 protocol such as TLS-AES-256-GCM-SHA384
- Add TLS 1.2 protocols such as TLS_ECDHE_ECDSA_WITH_AES_256_GCM_SHA384 and TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384
- Add new TLS API(s) to create TLS session without a connected TCP socket

## Features

This NetXsecure library provides support for WPA3-Enterprise security

## Enabling NetXSecure library
Update the below lines in Makefile

`#COMPONENTS=` 
to
`COMPONENTS+=NETXSECURE_WPA3`

`#DISABLE_COMPONENTS=`
to
`DISABLE_COMPONENTS+=NETXSECURE_ROM`

### Building the project
`make getlibs`

`make build -j8`

## Requirements

- [ModusToolbox® software](https://www.infineon.com/cms/en/design-support/tools/sdk/modustoolbox-software) v3.1

- Programming Language: C

## Supported Software and Tools
ToolChain | OS
----------|-----------------------
GCC_ARM   | AzureRTOS
----------------------------------

All other trademarks or registered trademarks referenced herein are the property of their respective owners.

-------------------------------------------------------------------------------

(c) 2021, Cypress Semiconductor Corporation (an Infineon company) or an affiliate of Cypress Semiconductor Corporation.  All rights reserved.
This software, associated documentation and materials ("Software") is owned by Cypress Semiconductor Corporation or one of its affiliates ("Cypress") and is protected by and subject to worldwide patent protection (United States and foreign), United States copyright laws and international treaty provisions. Therefore, you may use this Software only as provided in the license agreement accompanying the software package from which you obtained this Software ("EULA"). If no EULA applies, then any reproduction, modification, translation, compilation, or representation of this Software is prohibited without the express written permission of Cypress.
Disclaimer: THIS SOFTWARE IS PROVIDED AS-IS, WITH NO WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, NONINFRINGEMENT, IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. Cypress reserves the right to make changes to the Software without notice. Cypress does not assume any liability arising out of the application or use of the Software or any product or circuit described in the Software. Cypress does not authorize its products for use in any products where a malfunction or failure of the Cypress product may reasonably be expected to result in significant property damage, injury or death ("High Risk Product"). By including Cypress's product in a High Risk Product, the manufacturer of such system or application assumes all risk of such use and in doing so agrees to indemnify Cypress against all liability.