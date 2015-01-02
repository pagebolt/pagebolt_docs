PageBolt Theme Quickstart (1.0)
=========================

Thank you for purchasing the PageBolt theme!

PageBolt is a simple, refreshing one page theme designed for developers, and editors, looking for the next big thing in content management. Moreover, PageBolt is one of the first commercial modern themes available for either platform!

Pagekit and Bolt , two of the most advanced CMS frameworks on the planet, are our CMS tools of choice. And they're fun to use! Available for Pagekit, Bolt v2 and HTML5.

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

--
====

Pagekit Installation
===============

Step 1: Folder Structure
---------------

```
-PageBolt_Pagekit
--pagebolt-docs (Quickstart)
--pagebolt-files (Pagekit)
--pagebolt-sql (SQL)
```

Step 2: Create Database
---------------

Create a database (the default username, password and dbname is 'pagebolt').

Import the included database file (**pagebolt-db.sql**) located in the 'pagebolt-sql' folder.

Be sure to take note of database username and password.

Step 3: Upload Files
---------------

The Pagekit installation files are located in the **'pagekit-files'** folder. It is necessary to apply the recommended file permissions and server instructions via Pagekit's website here - http://www.pagekit.com/docs/troubleshooting


Step 4: Edit Config
---------------

Pagekit's configuration is stored in config.php in the Pagekit root folder (**pagebolt-files**). Here you will find the database credentials. Replace DBNAME, USERNAME and PASSWORD accordingly.

```
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

Once the installation was successful you can log in to Pagekit's control panel via the login screen by appending **/admin** to your URL with the default account credentials:

**Username**: pagebolt, **Password**: pagebolt

**IMPORTANT**: Be sure to change the theme's default username, password and email.

Step 6: Template Sections
---------------

All template sections, which are rendered with Razr templating, are all controlled via **'Widgets'**. The 'Terms and Conditions' and 'Privacy Policy' are the only actual 'Pages'. For your customization, the PageBolt theme is directly accessible in Pagekit's 'theme' directory. Visit the Pagekit website for more information on themes - http://www.pagekit.com/docs/themes

**Available Sections (edit the theme.php file for custom sections):**


```
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

Step 7: Installation Complete! Have Fun ;)
---------------
--
---------------

Bolt v2 Installation
===============

Step 1: Folder Structure
---------------

```
-PageBolt_Pagekit
--pagebolt-docs (Quickstart)
--pagebolt-files (Pagekit)
--pagebolt-sql (SQL)
```

Step 2: Create Database
---------------

Create a database (the default username, password and dbname is 'pagebolt').

Import the included database file (**pagebolt-db.sql**) located in the 'pagebolt-sql' folder.

Be sure to take note of database username and password.

Step 3: Upload Files
---------------

The Pagekit installation files are located in the **'pagekit-files'** folder. It is necessary to apply the recommended file permissions and server instructions via Pagekit's website here - http://www.pagekit.com/docs/troubleshooting


Step 4: Edit Config
---------------

Pagekit's configuration is stored in config.php in the Pagekit root folder (**pagebolt-files**). Here you will find the database credentials. Replace DBNAME, USERNAME and PASSWORD accordingly.

```
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

Once the installation was successful you can log in to Pagekit's control panel via the login screen by appending **/admin** to your URL with the default account credentials:

**Username**: pagebolt, **Password**: pagebolt

**IMPORTANT**: Be sure to change the theme's default username, password and email.

Step 6: Template Sections
---------------

All template sections, which are rendered with Razr templating, are all controlled via **'Widgets'**. The 'Terms and Conditions' and 'Privacy Policy' are the only actual 'Pages'. For your customization, the PageBolt theme is directly accessible in Pagekit's 'theme' directory. Visit the Pagekit website for more information on themes - http://www.pagekit.com/docs/themes

**Available Sections (edit the theme.php file for custom sections):**


```
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

Step 7: Installation Complete! Have Fun ;)
---------------

References
===============

* **Kube Framework** http://www.imperavi.com/kube/
* **Pagekit** http://www.pagekit.com/
* **Bolt** https://bolt.cm/
* **PageBolt Docs on Github** https://github.com/pagebolt/pagebolt_docs
