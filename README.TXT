<p>Welcome to Brutus theme's. An agile, powerful, easy and accessible theme for theme developers.</p>

<p>The main reason for the Brutus theme development is to make the work easier for themer developers.</p>

<p>After many years using Zen, 960 and Fusion themes, tuning and customizing them I have developed a new theme that provides an agile, powerful, easy and accessible theme development.</p>

<h2>Installation</h2>

- Download Brutus from http://drupal.org/project/brutus
- Unpack the downloaded file and place the Brutus folder in your Drupal installation under 
  one of the following locations:

    * sites/all/themes
    * sites/default/themes
    * sites/example.com/themes 

- Log in as an administrator on your Drupal site and go to 
  Administer > Site building > Themes (admin/build/themes) and make Basic the default theme.

- If you want to change the name of the theme from 'brutus' to another name like 'mytheme',
follow these steps (to do BEFORE enabling the theme) :


    - Edit brutus.info and change the name, description, project (can be deleted)

    - In brutus.info, replace the following instances of "brutus_" to "mytheme_"

      - [brutus_zen_tabs]
      - [brutus_block_editing]
      - [brutus_breadcrumb]
      - [brutus_breadcrumb_separator]
      - [brutus_breadcrumb_home]
      - [brutus_breadcrumb_trailing]
      - [brutus_breadcrumb_title]
	  
    - In template.php change each iteration of 'brutus' to 'mytheme'
    - In theme-settings.php change each iteration of 'brutus' to 'mytheme'
	- rename the theme folder to 'mytheme'
	- rename brutus.info to mytheme.info


<h2>Main folder description</h2>

- brutus.info => Provides informations about the theme, like regions, css, settings, js ...
- images => Image and graphic resorces folder
- js => Javascript files folder
	- browser.js => (http://rafael.adm.br/css_browser_selector/) Provides classes on HTML tags
	- equalHeight.js => Equal block height function
- css => CSS files folder
	- ie => Internet Explorer CSS files folder
		- ie6.sass => Used to debug IE6
		- ie7.sass => Used to debug IE7
	- partials => This folder will make our work easier
		- _header.sass => Header style file
		- _footer.sass => Footer style file
		- _grid.sass => Grid structure sile
		- _info.sass => Main info file
		- _reset.sass => Reset file
		- _skinr.sass => User friendly interface file
		- _tabs.sass => ZEN tabs file
		- _layout.sass => Layout settings and grid definition file
	- brutus.css.sass => Our custom CSS file
- logo.png => Logo file
- templates => Template files folder. One template file for each element
	- block.tpl.php => Template fantastic to edit the blocks
	- node.tpl.php => Template fantastic to edit the nodes
	- page.tpl.php => Template fantastic to edit the page
- template.php => Used to modify drupal's default behavior before outputting HTML through the theme
- theme-settings => Used to create additional settings in the theme settings page


*config.rb => Theme definition after compilation

mm-build and our theme will be created

<h2>Final project folder description</h2>

- brutus.info => provide informations about the theme, like regions, css, settings, js ...
- images => Image and graphic resorces folder
- js => Javascript files folder
	- browser.js => (http://rafael.adm.br/css_browser_selector/) Provides classes on HTML tags
	- equalHeight.js => Equal block height function
- css => CSS files folder
	- ie => Internet Explorer CSS files folder
		- ie6.css => Used to debug IE6
		- ie7.css => Used to debug IE7
	- brutus.css => Final CSS file with all the stuff (compressed and without comments if you wish. You could custom generate it)
- logo.png => Logo file
- templates => Template files folder. One template file for each element
	- block.tpl.php => Template fantastic to edit the blocks
	- node.tpl.php => Template fantastic to edit the nodes
	- page.tpl.php => Template fantastic to edit the page
- template.php => Used to modify drupal's default behavior before outputting HTML through the theme
- theme-settings => Used to create additional settings in the theme settings page



Changing the Layout

The layout used in Brutus is fairly similar to the Holy Grail method. It has been tested on all major browser including IE (5>8), Opera, Firefox, Safari, Chrome ...
The purpose of this method is to have a minimal markup for an ideal display. 
For accessibility and search engine optimization, the best order to display a page is the following :

	1. header
	2. menu
	2. content
	3. sidebars
	4. footer


Thanks for using BRUTUS, and remember to use the issue queue in drupal.org for any question or bug report:

http://drupal.org/project/issues/brutus

Current maintainers:
* Neftalí Guerrero (nguerrero) - http://drupal.org/user/370767
