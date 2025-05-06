<!-- START doctoc generated TOC please keep comment here to allow auto update -->

- [Tizen studio for windows](#Tizen-for-windows)
  - [Download](#download)
  - [Package Manager](#package-manager)
  - [Config Tizen Studio](#config-tizen-studio)
  - [Config TV](#config-tv)
  - [Install Certificate](#install-certificate)
  - [Import App](#import-app)
  - [Build And Run](#build-and-run)
  - [Change URL](#change-url)
  - [Debug manager](#enable-manager)



<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# Tizen Studio for windows

`Tizen-for-windows` In this document you will find the steps to follow to install and configure Tizen Studio for the Windows operating system.


## Download

You can download the .exe file from the following link. [Tizen 6.1 Download](https://developer.tizen.org/development/tizen-studio/download/)

![Screenshot 2025-05-05 at 5 16 01 PM](https://github.com/user-attachments/assets/8d6f05ba-ebab-4b7e-a97d-10004eac42ca)

## Install

Open and install the .exe file.

![Screenshot 2025-05-05 at 5 17 52 PM](https://github.com/user-attachments/assets/84b0aa32-98bb-4b33-b2fd-0f71ba7ac908)

This should be a straightforward installation.

Next > OK > Etc.

When the installation is complete, make sure you have the Launch the Package Manager checkbox checked.

![Screenshot 2025-05-05 at 5 19 45 PM](https://github.com/user-attachments/assets/15f68fb8-d002-42f8-b9f8-2b3273447d0d)

## Package Manager

In this section, please install the following:
- Tizen 9.0
- Tizen 8.0
- Tizen SDK Tools
- Extras > TV Extensions-9.0

![Screenshot 2025-05-05 at 5 22 07 PM](https://github.com/user-attachments/assets/726699d6-ac83-424b-98ad-cb6ffd3cc83c)

Please note that TV Extensions-9.0 can be found under the Extras tab.

When you close the Package Manager application, please select the option: Launch Tizen Studio.

![Screenshot 2025-05-05 at 5 27 04 PM](https://github.com/user-attachments/assets/d35719eb-a6d9-4b6c-9699-ca4c08d0ae19)



## Config Tizen Studio

When you open Tizen Studio for the first time, you should set the workspace folder. (It's recommended to leave the default folder).


![Screenshot 2025-05-05 at 5 28 24 PM](https://github.com/user-attachments/assets/eba5b61f-358a-410b-94dd-f5571fb7bd9b)


## Config TV

In the next Select, please choose the option: Launch Remote Device Manager


![Screenshot 2025-05-05 at 5 30 44 PM](https://github.com/user-attachments/assets/bab811fe-c14b-466d-a70e-cf8306a17453)

Select the **Scan** option.

Once you find your device, click the Connect toggle.

![Screenshot 2025-05-05 at 5 32 55 PM](https://github.com/user-attachments/assets/2e048ed9-7e30-43ba-8105-2b5358e1130a)

**Remember that your TV and computer must be connected to the same network.**

**Also, remember that your TV must have your computer's IP address configured.**

In [this video](https://www.youtube.com/watch?v=F8kkdIh1TGY) you can see how to configure your computer's IP on your TV.

The command to see your IP in Windows is: **ipconfig**

You can run this command in a terminal and you will see your IP address.


![Screenshot 2025-05-05 at 5 36 07 PM](https://github.com/user-attachments/assets/458657f8-76cc-4e02-a6da-986d2887fc1e)

In theory, the **IPv4** address is the one you should configure in the developer mode section of your TV.

After you have connected your computer to your TV, you will see it reflected in the list.

![Screenshot 2025-05-05 at 5 38 05 PM](https://github.com/user-attachments/assets/83f35157-69d7-4e7b-818c-cad1ef1fa9d6)

## Install Certificate

A Samsung Tizen certificate is a profile that contains certificates needed to sign Tizen apps.

So, lets go to create our certificate. 

![Screenshot 2025-05-06 at 7 25 02 PM](https://github.com/user-attachments/assets/15327f72-627b-4815-bbf7-b77d0899ce3c)

In this section we are going to create a new certificate.


<img width="597" alt="Screenshot 2025-05-06 at 7 47 23 AM" src="https://github.com/user-attachments/assets/08d954c6-e965-44c2-8193-4035b6be9769" />

Please set any name.

<img width="597" alt="Screenshot 2025-05-06 at 7 49 08 AM" src="https://github.com/user-attachments/assets/7a04c020-8653-410e-9c2a-64b910f22df1" />

In the certified author section, we will select the option Select an existing author certificate and upload the author.pwd file.
(You should have this file; for security reasons, it will not be added to this repository. If you don't have this file, please contact me).


<img width="604" alt="Screenshot 2025-05-06 at 7 53 46 AM" src="https://github.com/user-attachments/assets/6f64373a-b3ca-460b-90f7-240e84245685" />

For the password field, please add the password shared with you.
(You should have this password; for security reasons, it will not be added to this repository. If you don't have this password, please contact me).

<img width="601" alt="Screenshot 2025-05-06 at 7 54 32 AM" src="https://github.com/user-attachments/assets/b60059ba-ac39-4bdc-9cdd-0180a38f3ae2" />

In the last section, Distributor certificate.
Let's select the second option: Select a distributor certificate for another app store.

![distributor first opt](https://github.com/user-attachments/assets/00bf57d1-4ee7-47ab-9b2e-4656a4f4097f)

Okay, now we're going to add the distributor.p12 file and put the shared password on the NFL team.

You should have both the file and the password. For security reasons, they will not be added to this repository.
If you don't have either of these, please contact me.

![image](https://github.com/user-attachments/assets/5776556b-b2d6-4003-b326-cf41e6daa46b)

Okay, we now have our certified profile.
Once you finish creating this profile, you should see something like this.


<img width="601" alt="Screenshot 2025-05-06 at 8 01 55 AM" src="https://github.com/user-attachments/assets/98891248-6de0-445e-b27a-e53ce98147de" />

## Import app

This section is quite simple, we are going to import the application from: File > Import


![import](https://github.com/user-attachments/assets/abe98c79-4bca-49e1-b7b0-9b83d27eb9e8)

We will select the Tizen Project option

![tizenproject](https://github.com/user-attachments/assets/33d7d3c0-47eb-4ca8-ae10-7111bf618dd5)

Our application is already compressed, we will select the option: Archive file

![archivefile](https://github.com/user-attachments/assets/14d1aacc-6958-448e-940e-d788f7acd2f9)

And here we'll upload the NFL_App.wgt file (you should have this file; for security reasons, it won't be uploaded to the repository. If you don't have it, please contact me)


![appwgt](https://github.com/user-attachments/assets/ab1980b5-9aca-4042-b84b-637d9046a7dc)

Ok, now we move on to a very important section: defining the project type.
In the Profile option, we'll select tv-samsung.
The version option should be 9.0.

Please enable the application check and click Finish.

(Remember that to configure the tv-samsung profile, you must have installed the necessary packages.)

![porfile](https://github.com/user-attachments/assets/e45f5bb8-3e33-4511-8bbe-57d2c578d511)

Once the project has been imported successfully, you should see it in the left menu.

![nflapp_project](https://github.com/user-attachments/assets/00bdd467-a6e2-4987-aec9-dc77ef15ec03)

## Build and Run 

This is the last section, here we will build and run the project on the TV.

To do this, we will right-click on the root folder of the project (in the left menu) and select the option: Build Signed Package)

![build1](https://github.com/user-attachments/assets/4e565fa6-3ba3-4616-913e-dd2796cf667e)

![build2](https://github.com/user-attachments/assets/37f8358a-b92a-47a4-9b15-f216a8800c84)

Once the build is complete (it's a fairly quick process), we'll see a new file inside our folder with the .wgt extension.
In this case, it's NFL_App.wgt.

Right-click on that file and select: Run As, Tizen Web Application.

![runapp](https://github.com/user-attachments/assets/6abf263d-8465-47e0-abf5-ce3bdc3454b7)

Remember that in order to run the application on your TV, it must already be configured and connected to your TV, as seen in the following image.

![connectedTV](https://github.com/user-attachments/assets/b4554391-1c42-4580-8302-3d53fdb91b7a)

## Change URL

In case you need to change the URL for a specific URL, just open the config.xml file by double clicking on it.

![configxml](https://github.com/user-attachments/assets/1a1355a0-ab20-4053-8031-9fbc3917c7d6)

Select the Source option and change the URL in the `<content ... />` tag.

![content](https://github.com/user-attachments/assets/bd53f390-a381-4567-a986-027c58a792e6)

Save with Ctrl + S.

## Debug Manager

To enable the debug manager option in our application, simply add the following string to the configured URL.
`&amp;debug=true`

Save with Ctrl + S.

![debug](https://github.com/user-attachments/assets/587ddb00-ff3f-4a23-9feb-0adc727b332d)
