---
title: Configuring ODK Collect for data collection
author: ~
date: '2018-04-30'
slug: configuring-odk-collect-for-data-collection
categories:
    - Data Collection
tags:
    - tutorials
    - open data kit
header:
  caption: ''
  image: ''
---

Once **ODK Collect** has been installed on the mobile device/s that you will be using for data collection, you may want to configure it's settings so as to be able to fully maximise its use and also to make it as easy as possible to use by your enumerators. Depending on how involved you aim your enumerators to be in the management of the data collection process, you may want to make available or limit certain settings or functions of **ODK Collect**.

This tutorial describes how to setup the various configuration options of **ODK Collect** with the aim of minimising possible unintended interference by enumerators on the various settings that might be detrimental to your data collection campaign. These include the options to load blank forms and change the settings of the server platform (if you are using any). This guide is aimed at IT administrators and/or survey coordinators/managers who will be setting up **ODK Collect** prior to distribution of the mobile devices to enumerators.

This tutorial assumes that **ODK Collect** is already installed on your mobile devices. The following <a href="http://sudan.validmeasures.org/installing-odk-collect-1/" target="_blank">tutorial</a> shows how to install **ODK Collect** on mobile devices.
<br />

## 1. Open ODK Collect
Find the **ODK Collect** app icon on your device and tap. You will see the following on your screen. This is the default configuration of ODK Collect when it is first installed on a device and the configurations have not been changed yet.
<img src="/img/tutorials/open-odk-collect.png" />
<br />

## 2. Tap on the ODK Collect settings menu
On the upper right hand corner, you will see three square dots on top of each other **(1)**. Click on this and a dropdown menu will appear showing options for ***'General Settings'*** **(2)** and for ***'Admin Settings'*** **(3)**.
<img src="/img/tutorials/tap-on-the-odk-collect-settings-menu.png" />
<br />

## 3. Tap on General Settings
First, we should configure the ***'General Settings'*** option of **ODK Collect**. This is what you will see once you tap on ***'General Settings'***.

There are three main 'General Settings' categories that can be configured: ***Server Settings*** **(1)**, ***Auto Send*** **(2)**, and ***User Interface*** **(3)**.
<img src="/img/tutorials/tap-on-general-settings.png" />
<br />

### 3.1 Configure Server settings
In ***'Server Settings'***, there are three main settings that will need configuring: ***Platform*** **(1)**, ***Platform settings*** **(2)** and ***Google account*** **(3)**.

First, tap on ***Platform*** **(1)**.
<img src="/img/tutorials/configure-server-settings.png" />
<br />

You will then be presented with various platform options that you can select depending on the type of server that you are using for your data collection campaign. **ODK Aggregate** is the default platform. For anything other than the default **ODK Aggregate** platform that is provided on **ODK Collect** by default, you will most likley need to select **Other** option so that you can specify your own platform for your data collection server.
<img src="/img/tutorials/31ef1184-ca3c-4bce-bc48-8c353c74c89c.png" />
<br />

Next, tap on ***'Configure platform settings'*** **(2)**.
<img src="/img/tutorials/a7f48316-38cf-4341-af23-43862b88ce14.png" />
<br />

You will then see the following options on your screen. Here you can specify the settings of the server used by your platform specifically the **URL of your server** **(1)**, the **username** **(2)** and **password** **(3)** use to login to your server. If you do not know these settings, you should ask your IT administrator or whoever setup your server platform to provide you with these settings. For most service providers offering servers for use by ODK, these settings are made explicit within your account so all you might need to do is to login to your account and find these settings.
<img src="/img/tutorials/88cfe68e-ce2c-4df7-8d57-f75de667a6f3.png" />
<br />

For example, if you are using a locally-deployed **Formhub** server as your **ODK** platform, you can find your server settings by logging in to your account and then scrolling down to the bottom of the webpage of the Formhub portal, you will see the following information about your Formhub server which you can use to setup the platform settings on your ODK Collect.
<img src="/img/tutorials/72c17efc-c1d2-409a-8670-f542ef7df08e.png" />
<br />

Next, configure your ***'Google accont'*** if you have one. This is not absolutely necessary and should be configured if you want to connect your **ODK Collect** with your **Google account** (if you have one). The advantage of doing this is that your data can be backed up to your **Google account**.
<img src="/img/tutorials/08563fc6-c78c-41d2-9fdd-73d6a0c4d0bf.png" />
<br />

### 3.2 Configure Auto Send settings
Now you can configure **Auto Send** settings. There are two settings to setup: ***'Auto send with Wi-Fi'*** **(1)** and ***'Auto send with network'*** **(2)**.

By default, these options are unchecked. It is recommended that you keep the default (unchecked) settings in place. This would mean that completed and finalised forms will be saved onto the device memory even when the device is connected on Wi-Fi and will not be sent unless the user specifically sends the forms for submission over the internet. It is good to have it this way because this allows for some type of checking of forms on the tablets themselves before they are sent to the server.
This is also good when there is no reliable Wi-Fi and/or network connection or if no server has been setup for the data collection campaign. The option to send the forms by Wi-Fi or over the network can be done later on when there is reliable network and/or when a server has been setup. Otherwise, manual sending of finalised forms via direct mobile device to computer connection can be done.
<img src="/img/tutorials/configure-auto-send-settings.png" />
<br />

### 3.3 Configure User Interface settings
Now you can configure the ***'User Interface'*** settings. Following are the settings that you can configure or change:

* ***Constraint processing behaviour***** (1)** - this is the option that determines how **ODK Collect** processes the check and constraints that have been specified in your form. There are two options here. The first option is for **ODK Collect** to process the constraints at the end of the form when you are about to finalise the form. The second option is for **ODK Collect** to process the constraints everytime you move to the next question in the form. The default behaviour is to process the constraints after every question. It is recommended that the default option be kept (Validate upon forward swipe).

* ***Navigation***** (2)** - this is the option that determines how the user can move from one question to the next in a form. The default behaviour is to use horizontal swipes. It is recommended that the option for use of forward/backward buttons be selected instead. Swiping is very user dependent and not all find it easy to use swiping gestures to move to the next question. Buttons, however, is universally acceptable and easy to train enumerators on using.

* ***Text font size***** (3)** - this is the option to change the font size used in **ODK Collect**. By default, this is set to Medium. This default is more than adequate and can be kept as is.

* ***Default to finalized***** (4)** - this is the option of whether all forms are by default finalized when you reach the end of the questionnaire. This is by default checked and when you reach the end of your questionnaire, you will see a prompt asking whether you want to mark the form as finalized and this option will be checked automatically because of this setting. It is recommended to keep this setting as is.

* ***Delete after send***** (5)** - this is the option of whether forms should be deleted after it has been sent to the server. By default this is unchecked. It is recommended that this option be kept unchecked as it is useful to have the forms kept on the devices as backup which can be retrieved later on manually via mobile device to computer connection as a form of backup. This is especially important in settings where internet is unreliable and that a backup of the data on the device is crucial.

* ***Enable hi-res video***** (6)** - this is the option of whether hi-res video playback is required. Unless you require video for your forms, it is recommended to uncheck this option.

* ***Show splash screen***** (7)** - this option determines if a splash screen on startup of **ODK Collect** should be shown. This option by default is turned off. It is recommended that this default is kept as is as there is no need for a splash screen and this only delays the startup of the **ODK Collect** application.

<img src="/img/tutorials/configure-user-interface-settings.png" />
<br />

## 4. Tap on Admin Settings
Now, you should configure the ***'Admin Settings'*** **(3)**.

The ***'Admin Settings'*** allow you to control what kinds of items are made available to the user of **ODK Collect**.
<img src="/img/tutorials/tap-on-admin-settings.png" />
<br />

### 4.1 Setting an Admin password
If you would like to block access to the ***'Admin Settings'*** on the **ODK Collect**, it would be recommended to set a password for access.
<img src="/img/tutorials/setting-an-admin-password.png" />
<br />

### 4.2 Form processing logic
***'Form processing logic'*** settings should be kept as default.
<img src="/img/tutorials/form-processing-logic.png" />
<br />

### 4.3 Configure User Can Access Main Menu Items settings
Now to configure the ***'User Can Access Main Menu Items'*** settings.

* ***Edit Saved Form***** (1)** - this is checked by default. Keep checked.

* ***Send Finalized Form***** (2)** - this is checked by default. Keep checked.

* ***Get Blank Form***** (3)** - this is checked by default. Uncheck this option. Unchecking this will hide it from the Main Menu. This will prevent unintended pulling of forms from the server that is not needed for your current data collection campaign.

* ***Delete Saved Form *****(4)** - this is checked by default. Uncheck this option. Unchecking this will hide is from the Main Menu. This will prevent unintended deletion of forms from the **ODK Collect**.

<img src="/img/tutorials/configure-user-can-access-main-menu-items-settings.png" />
<br />

### 4.4 Configure User Can Access Change Settings Items settings
Now, configure the ***'User Can Access Change Settings Items'*** settings.

The first five settings are shown here **(1-5)**. It is recommended that all of these be unchecked to avoid unintend changing of settings.
<img src="/img/tutorials/configure-user-can-access-change-settings-items-settings.png" />
<br />

The next set of settings are shown here **(6-14)**. All these settings should be unchecked except for ***'Text font size'***. This will avoid unintended changing of settings.
<img src="/img/tutorials/a9e43315-b32f-48b0-a0eb-074265679696.png"` />
<br />

### 4.5 Configure User Can Access Form Entry Items settings
Now you can configure ***'User Can Access Form Entry Items'*** settings.

The settings are shown below **(1-6)**. All options should be kept checked except for ***'Name this Form'*** which should be unchecked.
<img src="/img/tutorials/configure-user-can-access-form-entry-items-settings.png" />
<br />

## 5. Reminders
You should configure the ***General Settings*** first before you change the ***Admin Settings***. This is because the menu items needed to configure General Settings will not be available to you anymore one you have changed the Admin Settings as per recommendation above.

This means you should also get the blank forms loaded onto **ODK Collect** already before changing the ***Admin Settings*** because you will not have the option to get blank forms once you have changed the ***Admin Settings***. However, if you need to load forms onto **ODK Collect**, you can still do so by transferring the **XForms** version of the form straight into the mobile device from your computer using a mobile device to computer connection. Or you can activate the ***Get Blank Forms*** option again so that you can pull the blank forms from your server.
