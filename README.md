# MuraBootstrap4 Bundle
A [Mura CMS](http://www.getmura.com) Site Bundle based on [Bootstrap](http://getbootstrap.com/), a responsive, mobile first front-end framework for faster and easier web development. This also includes [Font Awesome](http://fontawesome.io/), the iconic font designed for Bootstrap.

## What Is A Mura CMS Site Bundle?
A site bundle for Mura CMS is a .ZIP file. There's no need to unzip it! The file contains data that has been exported from the database, as well as all of the assets used for the site such as images, CSS, JavaScript, and of course any layout templates used by the originating site.

A site bundle is a convenient way to share a custom theme and populate the site with some sample content to help other developers get up and running quickly and easily. Smaller sites often use bundles as backup files. This also makes it easy to work on a site locally on your laptop, and then re-deploy the site to the production server when finished.

## How To Install A Mura CMS Theme Bundle
1. From the Github project page, click the **Download ZIP** button located on the bottom, right column area.
2. Unzip the contents to reveal a file named as:
	**MuraBundle\_{ThemeName}\_YYYY\_MM\_DD\_HH\_MM.zip**
3. Login to the back end Admin area of the site where you wish to deploy the bundle.
4. Go to **Site Config > Deploy Bundle**
5. The first option listed is **Are you restoring a site from a backup bundle?**
	1. The default option is **No - Assign New Keys to Imported Items**. Unless you are actually restoring a site from a backup bundle, you should use this option.
	2. IF, and only if, you are restoring a site from a backup bundle, then you should select **Yes - Maintain All Keys from Imported Items**. However, you MUST be deploying the bundle to the same site. Do NOT attempt to deploy the bundle file with this option to a new site under the same instance of Mura.
6. Under the **Include:** option, you can select the various data you wish to import such as:
	1. Site Architecture & Content (_this is very common_)
	2. Site Members & Administrative Users
	3. Mailing List Members
	4. Form Response Data
	5. All Plugins
7. The next option is **Which rendering files would you like to import?**. You may select either **All**, **Theme Only**, or **None**. Typically, you would want to select either All, or Theme Only.
8. Next, select only one of the next two options:
	1. **Select Bundle File From Server (Preferred)**
		1. This is the recommended option. First, you must FTP the bundle file to a location under the Mura webroot. For example: ```/wwwroot/temp/```. Then, click the **Browse Server** button, navigate to the location where the file resides, and select it.
	2. **Upload Bundle File**
		1. For very small bundle files, this option may work without any issues. However, many browsers and web servers have filesize limits when submitting a form. Many bundles exceed the filesize restriction, so it is recommend to use the first option whenever possible.
9. Click **Update**

## License
Copyright 2014-2016 Blue River Interactive Group, Inc.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this work except in compliance with the License. You may obtain a copy of the License in the LICENSE file, or at:

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
