# InstagramFeed
Magento 2 Instagram Feed  is a supportive module which allows integrating Instagram images to Magento 2 website by allowing us to insert as widget in frontend. This uses cron to fetch images from instagram API and store it locally to avoid performance delay due to directly accessing insta images via API on the fly.
## Install via Composer (recommended)

Run the following command in Magento 2 root folder:

```
composer require ziffity/module-instagramfeed
php bin/magento setup:upgrade
php bin/magento setup:static-content:deploy
```
## Configuration


Open the Magento 2 Admin Panel and navigate to:

**Stores > Settings > Configuration > Ziffity > Instagram Feed**

<img src="images/Screenshot from 2022-02-27 22-21-24.png"/>

Available Configurations

### Available Configuration
#### 1.1 Insatgram Settings

##### Enable

Enable or disable the Instagram feed.

##### User Token (Required)

Instagram API USer token, required by Instagram to display your feed.

To create User token refer this <a href="https://www.mageplaza.com/kb/how-to-get-instagram-feed-access-token.html" target="_blank">link</a><br>
Note: Skip "Client OAuth Setting" steps for local testing.

#### 1.2 Insatgram Display Settings

##### Total number of photos

Insert the number of pictures that will be presented on feed
(The maximum value for the number of pictures is 25)

##### Hashtag Filter
Filter Images those will be presented on feed
Enter comma seperated hashtag Ex: NewYear,Christmas,Easter

##### Cron Setting
Customize cron Schedule time

##### Enable Log
Display logs for Debugging Purpose

##### Number of rows
Insert number of rows to be displayed

## Instagram Widget


Open the Magento 2 Admin Panel and navigate to:

**Content  > Widget > Add Widget**

Choose Type (Ziffity Instagram) and Current theme then click continue.

Configure storefront properties

Ex:
   Layout updates:

         Display on : All pages

         Cotainer: Page Footer

   For above configuration the output instagram post images with slider will be shown in footer section of all pages

   While clicking that image it will direct to corresponding insta post page

   <img src="images/frontend.png">















