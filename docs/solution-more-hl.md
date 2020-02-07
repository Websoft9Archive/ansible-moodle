# More

Each of the following solutions has been proven to be effective and we hope to be helpful to you.

## Domain binding

The precondition for **Domain binding** is have completed the **Domain resolution** for Moodle Instance.

From the perspective of server security and subsequent maintenance considerations, the **Domain Binding** step cannot be omitted.

Moodle domain name binding steps:

1. Connect your Cloud Server
2. Modify [vhost configuration file](/stack-components.md#apache), change the domain name item for you
   ```text
   #### Moodle (LAMP) bind domain #### 

     <VirtualHost *:80>
     ServerName www.mydomain.com # modify it for you
     DocumentRoot "/data/wwwroot/moodle"
     ...
     
   #### Moodle (LEMP) bind domain #### 

     server {
      listen 80;
      server_name    moodle.example.com; # modify it for you
     ...

   ```
3. Save it and restart [Web Service](/admin-services.md#apache)


## Register your Moodle site

Once completed your Moodle installation wizard, suggest you to register Moodle's website account. This account can help you to get upgrade message, get share course of Moodle.NET, install plugins online

1. Log in Moodle console as administrator
2. Open **Site administrator** > **Registation**
   ![Moodle register](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/moodle-registermd-websoft9.png)
3. When you completed it, Moodle.net may stay in touch and provide you with important things for your Moodle site

## Moodle languages

1. Log in Moodle console as administrator
2. Open **Site administrator** > **Language**
   ![Moodle language setting](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/moodle-languageset-websoft9.png)
3. Set it by yourself
   * Language settings: choose your language online
   * Language customisation: edit your language files online
   * Language packs: upload your language packs

## Moodle mobile

1. Log in Moodle console as administrator
2. Open **Site administrator** > **Mobile app** > **Mobile settings**
   ![moodle-apps](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/moodle-app-1-websoft9.png)
3. Check **Enable web services for mobile devices** is selected
   ![moodle-apps](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/moodle-app-2-websoft9.png)
4. Save settings
5. Install [Moodle APPS](https://download.moodle.org/mobile/) in your phone
6. Open the Moodle app in your phone, configure the Moodle's URL to your app and start to use it
   ![moodle-apps](https://libs.websoft9.com/Websoft9/DocsPicture/zh/moodle/moodle-mobile-websoft9.png)

## Moodle plugins

Moodle is very scalable platform, most of function were as plugins. Moodle have installed 400+ plugins by default and you can install plugins from [Plugins Marketplace](https://moodle.org/plugins/) to extend your functions

1. Log in Moodle console as administrator
2. Open **Site administrator** > **Plugins** 
   ![moodle plugins](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/moodle-plugins-websoft9.png)
3. Click **Plugins Overview** to list all plugins installed, you can disable and uninstall it also
4. Visit [Plugins Marketplace](https://moodle.org/plugins/) to search more plugins
5. Start to install plugins in the Moodle's console
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/moodle-intallplugins001-websoft9.png)
6. Upload plugin online
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/en/moodle/moodle-intallplugins-uploadfile-websoft9.png) 

> More details about manage plugins please refer to official docs [Moodle Plugins](https://docs.moodle.org/37/en/Installing_plugins)
