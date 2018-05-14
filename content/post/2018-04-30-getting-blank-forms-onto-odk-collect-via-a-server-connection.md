---
title: Getting blank forms onto ODK Collect via a server connection
author: ~
date: '2018-04-30T11:25:00'
slug: getting-blank-forms-onto-odk-collect-via-a-server-connection
categories:
    - Data Collection
tags:
    - tutorials
    - open data kit
header:
  caption: ''
  image: ''
---

To be able to use **ODK Collect** for data collection, pre-designed data collection forms will have to be loaded onto the application. There are generally two ways of performing this task.

* Get blank forms from a pre-configured **ODK server** designed to distribute blank forms and also to receive form submissions; and,

* Get blank froms directly onto the mobile device via a USB connection with a computer where the pre-designed data collection forms are located.

This tutorial describes how to get blank forrms onto **ODK Collect** through a pre-configured **ODK server**. This tutorial is applicable for web-based or cloud-based **ODK servers** such as <a href="https://formhub.org" target="_blank">Formhub</a>, <a href="http://www.surveycto.com/index.html" target="_blank">SureyCTO</a>, <a href="http://www.kobotoolbox.org" target="_blank">KoBoToolbox</a>, <a href="https://ona.io" target="_blank">ONA</a> or <a href="https://opendatakit.org/use/aggregate/" target="_blank">ODK Aggregate</a> or for variants of these servers that are locally-deployed (i.e., server installed onto a local computer). This tutorial assumes that you:

* Have an account with one of the web-based or cloud-based **ODK servers** or that you have your own web-based deployment of one of these **ODK servers** or its variants or that you have your own locally-deployed **ODK server**;

* <span style="color: rgb(1,24,55)">Have created forms using the </span><span style="color: rgb(1,24,55)">**XLSForm**</span><span style="color: rgb(1,24,55)"> standard. Instructions and guide on how to create forms using </span><span style="color: rgb(1,24,55)">**XLSForm**</span><span style="color: rgb(1,24,55)"> standard can be found </span><span style="color: rgb(142,190,218)"><a href="http://xlsform.org/">here</a></span><span style="color: rgb(1,24,55)">. If you have created forms using </span><span style="color: rgb(1,24,55)">**XForms**</span><span style="color: rgb(1,24,55)"> standard, consider using the second approach of transferring blank forms directly onto mobile device via a USB connection with a computer;</span>

* <span style="color: rgb(1,24,55)">Have uploaded your forms onto your </span><span style="color: rgb(1,24,55)">**ODK server**</span><span style="color: rgb(1,24,55)">. A tutorial on how to upload forms onto an </span><span style="color: rgb(1,24,55)">**ODK server**</span><span style="color: rgb(1,24,55)"> can be found </span><span style="color: rgb(1,24,55)"><a href="http://sudan.validmeasures.org/publishing-forms-onto-formhub-local-server/" target="_blank">here</a></span><span style="color: rgb(1,24,55)">;</span>

* <span style="color: rgb(1,24,55)">Have internet access (for web-based </span><span style="color: rgb(1,24,55)">**ODK servers**</span><span style="color: rgb(1,24,55)">) or a local area network configured (for locally-deployed </span><span style="color: rgb(1,24,55)">**ODK servers**</span><span style="color: rgb(1,24,55)">); and,</span>

* <span style="color: rgb(1,24,55)">Have </span><span style="color: rgb(1,24,55)">**ODK Collect**</span><span style="color: rgb(1,24,55)"> installed on your mobile device. </span>

Now, let's get blank forms onto your mobile device.

## 1. Open ODK Collect
Find the **ODK Collect** app icon on your device and tap. You will see the following on your screen.
<br />

<img src="/img/tutorials/open-odk-collect.png" />
<br />

## 2. Configure ODK Collect server settings
On the upper right hand corner of the **ODK Collect** screen, you will see three square dots on top of each other **(1)**. Click on this and a dropdown menu will appear showing options for ***'General Settings'*** **(2)** and for ***'Admin Settings'*** **(3)**.
<br />

<img src="/img/tutorials/configure-odk-collect-server-settings.png" />

### 2.1 Tap on General Settings
First, we should configure the ***'General Settings'*** option of **ODK Collect**. This is what you will see once you tap on ***'General Settings'***.

There are three main 'General Settings' categories that can be configured: ***Server Settings*** **(1)**, ***Auto Send*** **(2)**, and ***User Interface*** **(3)**.
<br />

<img src="/img/tutorials/tap-on-general-settings.png" />
<br />

### 2.2 Tap on server settings
In ***'Server Settings'***, there are two main settings that will need configuring: ***Platform*** **(1)** and ***Platform settings*** **(2)**.

First, tap on ***Platform*** **(1)**.
<br />

<img src="/img/tutorials/tap-on-server-settings.png" />
<br />

You will then be presented with various platform options that you can select depending on the type of server that you are using for your data collection campaign. **ODK Aggregate** is the default platform. For anything other than the default **ODK Aggregate** platform that is provided on **ODK Collect** by default, you will most likely need to select **Other** option so that you can specify your own platform for your data collection server.
<br />

<img src="/img/tutorials/7893044c-9d57-4395-8b68-853ed56bebf5.png" />
<br />

Next, tap on ***'Configure platform settings'*** **(2)**.
<br />

<img src="/img/tutorials/7298b62a-d734-49a9-b1b6-8f0d6d4baeb6.png" />
<br />

You will then see the following options on your screen. Here you can specify the settings of the server used by your platform specifically the **URL of your server** **(1)**, the **username** **(2)** and **password** **(3)** used to login to your server. If you do not know these settings, you should ask your IT administrator or whoever setup your server platform to provide you with these settings. For most service providers offering servers for use by ODK, these settings are made explicit within your account so all you might need to do is to login to your account and find these settings.
<br />

<img src="/img/tutorials/bb41af04-0c2d-4a35-873d-65783400301e.png" />
<br />

For example, if you are using a locally-deployed **Formhub** server as your **ODK** platform, you can find your server settings by logging in to your account and then scrolling down to the bottom of the webpage of the Formhub portal, you will see the following information about your Formhub server which you can use to setup the platform settings on your ODK Collect.
<br />

<img src="/img/tutorials/0f69dcbf-841f-4fcf-a113-b010e4bc7016.png" />
<br />

## 3. Get blanks forms from the server
Once you have configured the server settings, go back to the main screen of **ODK Collect** (as shown below) and then tap on ***'Get Blank Form'***.
<br />

<img src="/img/tutorials/get-blanks-forms-from-the-server.png" />
<br />

You will then see a list of the various blank forms that are available from the server. In the example below, there is only one form available called **Incidence / ****حدوث**.

Select this form by ticking the box on its right hand side ***(1)***. Then tap the button on the bottom right hand corner of the **ODK Collect** screen labeled ***'Get selected' *****(2)**.
<br />

<img src="/img/tutorials/3bbba33a-8611-48ea-b4a9-a6f4b5220f1e.png" />
<br />

You will then see the following prompt indicating that **ODK Collect** is communicating with the server and downloading the **Incidence / ****حدوث** blank form.
<br />

<img src="/img/tutorials/f1845190-e09f-42ff-98c8-88e7154c90bc.png" />
<br />

The following prompt will come out on your screen once the download process is finished.

Congratulations, you have successfully downloaded a blank form from your specified server!
<br />
