Jenkins-PHP + Symfony
=====================


Directions
----------
1. Clone this repo or Download the tarball.
2. Copy the app directory and build.xml into your Symfony root directory.
3. Enjoy.

*NOTE: You'll probably want to add "build/\*" to your SCM's ignore file.*

Things you may want to tweak
----------------------------
* PHP CodeSniffer Standard: Currently the default value (PEAR) set by PHP Project Wizard.
* PHPMD Rules: Currently the default value (codesize,design,naming,unusedcode) set by the PHP Project Wizard.

Credits
-------
* The initial build script was generated by [PHP Project Wizard](https://github.com/sebastianbergmann/php-project-wizard "PHP Project Wizard")
    * It's been modified to run phpunit from the app directory.
* The initial phpunit.dist.xml came with [Symfony](http://symfony.com/ "Symfony Framework") 2.0.3.
    * It's been modified to include a logging target that the build tools expect to exist.  
    * This target was provided by [Jenkins-PHP](http://jenkins-php.org/) and was modified to reflect the location of the build directory relative to the app directory