# Drupal Headless
Headless drupal means drupal without head { frontend }. Drupal backend as **{ PRODUCER }** provides ReSTful APIs for different clients **{ CONSUMERS }**. For example {Angular, ReactJs, VueJs, Android, iOS, ReactNative, Flutter }. Headless Drupal allows frontend developer and backend developer to work separately.

![headless](https://github.com/arsibux/drupal-headless/blob/main/_drawio/img/headless.drawio.png)

- **INSTALLATION**
- **CORE MODULES**
- **CONTRIB MODULES**
- **AUTHENTICATION**
  - **Basic Authenticaion**
  - **JWT Authentication**
- **REST RESOURCES**
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


- Install DEV Tools
  - Run `ddev ssh`.
  - Run `composer require --dev drush/drush`.
  - Run `composer require --dev drupal/devel`.
  - Run `composer require --dev drupal/webprofile`.
  - Run `composer require drupal/admin_toolbar`.

- Enable DEV modules.
  - Run `Drush pm:en devel devel_generate webprofile admin_toolbar`.
# Resources

# Changelogs
- 17-FEB-2023
  - ADDED: Definition Headless
  - ADDED: Installations
  - ADDED: Core and contrib module installation
  - ADDED: Configuration