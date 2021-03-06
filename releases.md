# Release Notes

- [Botble 3.3](#version_3_3)
- [Botble 3.2.1](#version_3_2_1)
- [Botble 3.2](#version_3_2)
- [Botble 3.2](#version_3_1)
- [Botble 3.0.2](#version_3_0.2)
- [Botble 3.0.1](#version_3_0.1)
- [Botble 3.0](#version_3_0)
- [Botble 2.6](#version_2_6)
- [Botble 2.5](#version_2_5)
- [Botble 2.4.2](#version_2_4_2)
- [Botble 2.4.1](#version_2_4_1)
- [Botble 2.4](#version_2_4)
- [Botble 2.3.1](#version_2_3_1)
- [Botble 2.3](#version_2_3)
- [Botble 2.2.1](#version_2_2_1)
- [Botble 2.2](#version_2_2)
- [Botble 2.1](#version_2_1)
- [Botble 2.0](#version_2_0)
- [Botble 1.0](#version_1_0)

<a name="version_3_3"></a>
## Botble 3.3
### 30-09-2018
- See what's new here: https://botble.com/whats-new-in-botble-cms-33

<a name="version_3_2_1"></a>
## Botble 3.2.1
### 22-06-2018

- Hotfix bulk actions and language column

<a name="version_3_2"></a>
## Botble 3.2
### 14-06-2018
- Fix bug UI & update admin UI
- Add Chinese language
- Refactor code & optimize queries
- Update vendor packages

<a name="version_3_1"></a>
## Botble 3.1
### 15-05-2018

- Support multi-language for theme options & widgets
- Fix bug add super users
- Upgrade table system & add filter tables
- Support change language on the login page
- Fix bug adding admin locale
- Fix bug create plugin by command

<a name="version_3_0_2"></a>
## Botble 3.0.2
### 12-04-2018

- Hotfix bug cannot create new custom field

<a name="version_3_0_1"></a>
## Botble 3.0.1
### 09-04-2018

- Fix bug cropping image size.
- Fix preview image in media management
- Move API clients to settings.
- Update UI for member frontend.
- Update UI in admin panel.

<a name="version_3_0"></a>
## Botble 3.0
### 04-04-2018

- Upgrade to Laravel 5.6 (change PHP required version to >=7.1.3)
- Add Passport support
- Refactor plugin system
- Refactor ACL system
- Fix bug member login and forgot password.
- Update UI
- Update some vendor packages

<a name="version_2_6"></a>
## Botble 2.6
### 21-02-2018

- Fix member reset password bug.
- Fix to change status after creating a new plugin.
- Auto register plugin menu to admin dashboard after creating new plugin.
- Update vendor packages.
- Fix coding standard.

<a name="version_2_5"></a>
## Botble 2.5
### 19-01-2018
- Update media module. Support Amazon S3 and allowing to upload video/mp4, support preview .mp4 video on admin panel.
- Allowing to add more extensions. Just need to add to .env file.
```
    RV_MEDIA_ALLOWED_MIME_TYPES=jpg,jpeg,png,gif,txt,docx,zip,mp3,bmp,csv,docs,xls,xlsx,ppt,pptx,pdf,mp4
```
- Fix admin menu with permissions.
- Fix some UI bugs.
- Add cache management. Now we can clear cache from admin panel.
- Upgrade custom field: Fix bugs, refactor code & adding import/export functions.

<a name="version_2_4_2"></a>
## Botble 2.4.2
### 29-12-2017
    - Refactor plugin language to make it easier to integrate with new plugin (check FAQ for more detail).
    - Fix bug when deleting default user `botble`.
    - Redirect back to previous page after login
    - Update default database.
    - Refactor slug plugin.

<a name="version_2_4_1"></a>
## Botble 2.4.1
    - Fix bug change profile image
    - Refactor plugin language & gallery
    - Move member to plugin
    - Update default database

<a name="version_2_4"></a>
## Botble 2.4
    - Upgrade to latest Laravel version 5.5. In this version, it's required PHP >= 7.0
    - Separate Admin users and members.
    - Update editor: allows multiple rich editor in a page, switch between text editor & rich editor.
    - Fix UI: dashboard widgets, plugins.

>  {warning} This a big update with Laravel framework, it's core update so to upgrade from version 2.3, you should copy your themes and plugins to version 2.4 and use new database from /database.sql.

<a name="version_2_3_1"></a>
## Botble 2.3.1
    - Fix create a Category.
    - Move analytics JSON config file to storage path.
    - Move repositories, criteria to support module.
    - Optimize media module.
    
<a name="version_2_3"></a>
## Botble 2.3
    - Apply new media management. There is many change on media on this version so the document for Media will be update later.
    - Add shortcode button above editor to easy add shortcode.
    - Allow switch between Ckeditor and Tinymce.
    - Fix bug when create new role.
    - Fix bug activate/deactivate user.
    - Add create user in admin area, now we have 2 options: create user and invite user.
    - Remove function get_file_by_size(). Now you can use get_image_url($post->image, 'thumb') instead of get_file_by_size.
    - Add front site users area.

<a name="version_2_2_1"></a>
## Botble 2.2.1
    - Add post format (Default, gallery, video...)
    - Fix bug in plugin language when default language is not set.
    - Change route name of post, page, category in front site from "public.view" to "public.single.detail"
    - Fix counter in Dashboard.
    - Refactor admin breadcrumb.
    - Set page title for each page in admin area.
    - Add new demo theme
    - Refactor show category list, theme list...
    - Remove admin bar config in theme
<a name="version_2_2"></a>
## Botble 2.2
    - Easier theme breadcrumbs. Now you can use Theme::breadcrumb()->add('label', 'http://...')->add('label2', 'http:...');
    - Fix invite user
    - Fix reset password
    - Update email template and send mail function.
    Now you can send mail by: `EmailHandler::send('Hello there', 'Test email', ['name' => 'Sang Nguyen', 'to' => 'sangit7b@gmail.com']);`
    - Remove laroute package.
    Please remove LarouteServiceProvider on /config/app.php and laroute package on composer.json.
    
<a name="version_2_1"></a>
## Botble 2.1

    - Upgrade to Laravel 5.4.
    - Upgrade custom field plugin
    - Refactor assets structure
    - Fix error when installing.
    - Fix analytics plugin after installation.

<a name="version_2_0"></a>
## Botble 2.0
### 11-09-2016
    - Fix https://github.com/botble/issues/issues/1: Media upload error
    - Please see image attachment in this issue to update your code.
    
### 11-08-2016
    - Fix installation script.

### 10-22-2016
    Release Botble version 2.0

<a name="version_1_0"></a>
## Botble 1.0 

### 09-13-2016
     - Fix folders in media is not accessible: To update, you just need update two files:
          + /resources/views/files/partials/folder-row.blade.php
          + /resources/views/files/partials/uplevel.blade.php
     - Fix Menu management: 
        Run "composer update" to update menu package or replace /vendor/botble/menu folder.

### 08-31-2016
    - Fix menu module (just run "composer update" to update menu module)
    - Fix media uploads:
        Replace botbe/repositories/feature, 
        app/http/controllers/features 
        and app/http/endpoints/feature, media.js in assets.

### 08-24-2016
    - Upgrade to Laravel 5.3

### 08-11-2016
    - Update routes and media

###  08-01-2016
    - Add social login (login to admin page via facebook, github, google...

### 07-16-2016
    - Add contact form support, fix some small bugs.

### 07-09-2016
    - Fix dashboard widget, custom field and media management.

### 07-08-2016
    - Initial release Version 1.0