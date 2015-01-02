PageBolt Theme Quickstart (1.0)
=========================

Thank you for purchasing the PageBolt theme! PageBolt is a simple, refreshing one page theme designed for developers, and editors, looking for the next big thing in content management. Moreover, PageBolt is one of the first commercial modern themes available for either platform! And they're fun to use. The PageBolt one-pager theme is available for Pagekit, Bolt v2 and HTML5.

**Features at a Glance:**

+ Built with Kube Framework
+ Responsive
+ Flexible Use of Content Types
+ Complete Use of Twig/Razr Templating
+ Dynamic Imagery via Velocity.js
+ Adaptive and Touch Ready
+ Retina Support
+ Quickstart Package
+ Free Updates
+ and much more!

**Server Requirements:**

+ Apache 2.2+ or Nginx
+ MySQL Server 5.1+
+ PHP Version 5.4+

**Links:**
* **Pagekit Demo:** http://www.pagebolt.io/
* **Bolt Demo:** http://bolt.pagebolt.io/
* **HTML5 Demo:** http://html5.pagebolt.io/
* **Follow Us On Twitter:** [@PageBolt](https://twitter.com/PageBolt)

*Current version: [v1.0]*



Pagekit Installation
===============

Step 1: Folder Structure
---------------

After downloading the package and unzipping it to your local server (i.e. WAMP, XAMPP, Vagrant), take a look at the folder structure and explore its contents.

```
-PageBolt_Pagekit
--pagebolt-docs (Quickstart)
--pagebolt-files (Pagekit)
--pagebolt-sql (SQL)
```

Step 2: Create Database
---------------

Create a database (the default username, password and dbname is 'pagebolt').

Import the included database file (**pagebolt-db.sql**) located in the **'pagebolt-sql'** folder.

**IMPORTANT:** Be sure to take note of database username and password.

Step 3: Upload Files
---------------

The Pagekit installation files are located in the **'pagebolt-files'** folder. It is necessary to apply the recommended file permissions and server parameters via Pagekit's website here - http://www.pagekit.com/docs/troubleshooting


Step 4: Edit Config
---------------

Pagekit's configuration options are stored inside the config.php file, which is located in the Pagekit root folder (**pagebolt-files**). Here you will find the database credentials. Replace DBNAME, USERNAME and PASSWORD accordingly.

```php
'database' => [
    'default' => 'mysql',
    'connections' => [
      'mysql' => [
        'host' => 'localhost',
        'user' => 'USERNAME',
        'password' => 'PASSWORD',
        'dbname' => 'DBNAME',
        'prefix' => 'pk_',
      ],
    ],
  ],
```

Step 5: Visit Admin URL
---------------

Once the installation was successful you can log into Pagekit's control panel via the login screen by appending **/admin** to your URL with the default account credentials:

**Username**: pagebolt, **Password**: pagebolt

**IMPORTANT**: Be sure to change the theme's default username, password and email!!

Step 6: Template Sections
---------------

All template sections, which are rendered with Razr templating, are all controlled via **'Widgets'**. For your customization, the PageBolt theme is directly accessible in Pagekit's **'themes'** directory. PageBolt's core theme template for Pagekit is located at **themes/pagebolt/templates/template.razr**. Visit the Pagekit website for more information on themes - http://www.pagekit.com/docs/themes

Learn more about Razr - https://github.com/pagekit/razr

**NOTE:** The 'Terms and Conditions' and 'Privacy Policy' are the only actual 'Pages'. Because of the single nature of one page themes, we use **/** as the home page within Pagekit.

**Available Sections (edit the theme.php file for custom sections):**


```php
// positions are sections in your theme where widgets can be published
'positions' => [
      'logo'            => 'Logo',
      'logo-small'      => 'Logo Small',
      'tagline'         => 'Tagline',
      'slider'          => 'Slider',
      'navbar'          => 'Navbar',
      'navbar-mobile'   => 'Navbar Mobile',
      'promo'           => 'Promo',
      'hero-box'        => 'Hero',
      'highlight-1'     => 'Highlight-1',
      'highlight-2'     => 'Highlight-2',
      'accordion'       => 'Accordion',
      'features'        => 'Features',
      'feature-1'       => 'Feature-1',
      'feature-2'       => 'Feature-2',
      'feature-3'       => 'Feature-3',
      'feature-4'       => 'Feature-4',
      'feature-5'       => 'Feature-5',
      'feature-6'       => 'Feature-6',
      'support'         => 'Support',
      'copyright'       => 'Copyright',
      'social'          => 'Social'
  ],
```

**Yay! Pagekit installation is now complete!**

Bolt v2 Installation
==============

Step 1: Folder Structure
---------------

After downloading the package and unzipping it to your local server (i.e. WAMP, XAMPP, Vagrant), take a look at the folder structure and explore its contents.

```
-PageBolt_Boltv2
--pagebolt-docs (Quickstart)
--pagebolt-files (Bolt)
--pagebolt-sql (SQL)
```

Step 2: Create Database
---------------

Create a database (the default username, password and dbname is 'pagebolt').

Import the included database file (**pagebolt-boltdb.sql**) located in the **'pagebolt-sql'** folder.

**IMPORTANT:** Be sure to take note of database username and password.

Step 3: Upload Files
---------------

The Bolt installation files are located in the **'pagebolt-files'** folder. It is necessary to apply the recommended file permissions and server parameters via Bolt's website here - https://docs.bolt.cm/installation


Step 4: Edit Config
---------------

Bolt uses YAML files for all configuration including content types. Bolt's database configuration is stored in **app/config/config.yml**, which is located in Bolt's /app folder (**pagebolt-files**). Here you will find the default database credentials. Replace DBNAME, USERNAME and PASSWORD accordingly.

```yml
database:
  driver: mysql
  username: USERNAME
  password: PASSWORD
  databasename: DBNAME
```

**NOTE:** The config file is in the YAML format, which means that the indentation is important. Make sure you leave leading spaces intact.

Step 5: Visit Admin URL
---------------

Once the installation was successful you can log into Bolt's control panel via the login screen by appending **/bolt** to your URL with the default account credentials:

**Username**: pagebolt, **Password**: pagebolt

**IMPORTANT**: Be sure to change the theme's default username, password and email!!

Step 6: Content Types
---------------

All Bolt template content types, which are rendered via the Twig templating engine, are all controlled by Twig template files located in **theme/pagebolt-bolt** folder. The key file is **theme/pagebolt-bolt/index.twig**, which includes the header and footer sections.

Content types are then easily managed in the Bolt administration panel. For your customization, the PageBolt theme is directly accessible via the **'File Management'** menu located in the Bolt admin panel. Visit the Bolt website for more information on themes - https://docs.bolt.cm/building-templates

It's about that time to pick up on **Twig** - http://twig.sensiolabs.org/

These are the main content types in the Bolt admin panel:

+ Tagline
+ Pages
+ Sections
+ Accordion
+ Features

**Available Content Types (edit the app/config/contenttypes.yml for customization):**


```yml
# PageBolt Tagline
tagline:
  name: Tagline
  singular_name: Tagline
  fields:
      title:
          type: text
          class: large
      slug:
          type: slug
          uses: [ title ]
      tagline:
          type: text
          label: PageBolt's Tagline
          height: 150px
          required: true
          postfix: "<p><em>Enter PageBolt's tagline.</em></p>"
  icon_many: "fa:quote-left"

# PageBolt Pages
pages:
  name: Page
  singular_name: Page
  fields:
      title:
          type: text
          class: large
    slug:
          type: slug
          uses: [ title ]
    content:
          type: html
          height: 300px
          postfix: "<p><em>Enter page content.</em></p>"
          required: true
  icon_many: "fa:file-text"
  template: page.twig

# PageBolt Sections
sections:
  name: Sections
  singular_name: Section
  fields:
      title:
          type: text
          label: Section Title
          class: large
          postfix: "<p><em>Enter PageBolt header title for section e.g. CMS Evolved</em></p>"
      slug:
          type: slug
          uses: [ title ]
      content:
          type: html
          height: 300px
          postfix: "<p><em>Enter section content.</em></p>"
          required: true
  icon_many: "fa:newspaper-o"
  sort: id
  recordsperpage: 20

#PageBolt Accordion
accordion:
  name: Accordion
  singular_name: Accordion
  fields:
      title:
          type: text
          class: large
          label: Accordion Title
          required: true
      slug:
          type: slug
          uses: [ title ]
      description:
          type: html
          label: Accordion Description
          height: 300px
          required: true
          record_template: entry.twig
  icon_many: "fa:th-list"
  sort: id
  recordsperpage: 20

#PageBolt Features
features:
  name: Features
  singular_name: Feature
  fields:
      title:
          type: text
          class: large
          label: Feature Title
          required: true
      slug:
          type: slug
          uses: [ title ]
      description:
          type: html
          label: Feature Description
          height: 300px
          required: true
          record_template: entry.twig
  icon_many: "fa:coffee"
  sort: id
  recordsperpage: 20
```

**Yay! Bolt installation is now complete.**

References
===============

* **Pagekit** http://www.pagekit.com/
* **Bolt** https://bolt.cm/
* **Kube Framework** http://www.imperavi.com/kube/
* **Razr** https://github.com/pagekit/razr
* **Twig** http://twig.sensiolabs.org/
* **PageBolt Docs on Github** https://github.com/pagebolt/pagebolt_docs
