SugarCRM CodeSniffer
====================


### Install PHP CodeSniffer

* 
  ```
  pear install PHP_CodeSniffer
  ```

### Install SugarCRM CodeSniffer

* 
  ```
  git clone git@github.com:svnvcristea/SugarCRMCodeSniffer.git
  ```

### Add SugarCS to the Standards

You have to copy the entire sub-folder SugarCS of this repo into the CodeSniffers Standards

* 
  ```bash
  cd ./SugarCRMCodeSniffer

  cp ./SugarCS   /usr/share/php/PHP/CodeSniffer/Standards/
  ```

### Add SugarCS to PHPStorm Inspections Profile
* in PHPStorm from *File/Settings/Editor/Inspections*
* on the same line with the Profile, click Manage/Import , select SugarCRM_Default.xml
* from the Profile now select *SugarCRM Default*

This will Runs PHP Code Sniffer to find coding style problems based on SugarCS standards

### Read more

SugarCS it's a standard based on PSR-2 with few exceptions. Read more about PSR-2 Coding Standards at:

* [PSR-2 Coding Style Guide](http://www.php-fig.org/psr/psr-2/)
* [Git pre-commit hook adjusted for SugarCRM CodeSniffer.](https://github.com/d-pluschaev/CsPCHookSugar)
