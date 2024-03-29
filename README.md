# Drupal Headless
Headless drupal means drupal without head { frontend }. Drupal backend as **{ PRODUCER }** provides ReSTful APIs for different clients **{ CONSUMERS }**. For example {Angular, ReactJs, VueJs, Android, iOS, ReactNative, Flutter }. Headless Drupal allows frontend developer and backend developer to work separately.

![headless](https://github.com/arsibux/drupal-headless/blob/main/_drawio/img/headless.drawio.png)

- **Installation**
- **Install Dev Tools**
- **Web Services Modules**
- **Authentication**
  - **Basic Authenticaion**
  - **JWT Authentication**
- **Rest Resources and Endpoints**
  - **Menus**
  - **Pages**
  - **Articles**
  - **Taxonomy**
  - **User Management**

## INSTALLATION

- Create working directory `mkdir headless-drupal` and `cd headless-drupal`.
- Run `ddev config --project-type=drupal10 --docroot=web --create-docroot`.
- Run `ddev composer create drupal/recommended-project` and select Yes.
- Run `ddev start`.
- Browse https://headless-drupal.ddev.site/
- Install drupal 10.

![installation](https://github.com/arsibux/drupal-headless/blob/main/_data/assets/images/installation-1.PNG)

## INSTALL DEV TOOLS
- Run `ddev ssh`.
- Run `composer require --dev drush/drush`.
- Run `composer require --dev drupal/devel`.
- Run `composer require --dev drupal/webprofile`.
- Run `composer require drupal/admin_toolbar`.
- Enable DEV modules run `drush pm:en devel devel_generate webprofile admin_toolbar`.

## WEB SERVICE MODULES
- Run this command to enbale core webservices modules  `drush pm:en basic_auth serialization rest`.
- Download contributed module {secured and stable version}.
  - Run `composer require drupal/restui` .
  - Run `composer require drupal/pager_serializer`.
  - Run `composer require drupal/rest_menu_items`.
  - Run `composer require drupal/jwt`.
- Enable modules run `drush pm:en restui pager_serializer rest_menu_items jwt`.

![webservice](https://github.com/arsibux/drupal-headless/blob/main/_data/assets/images/webservices.PNG)

## AUTHENTICATION
Takes a username and password out of the request and authenticates them against Drupal.
# Resources

# Changelogs
- 17-FEB-2023
  - ADDED: Definition Headless
  - ADDED: Installations
  - ADDED: Core and contrib module installation
  - ADDED: Configuration
- 18-FEB-2023
  - ADDED: Basic Authentication.
  -