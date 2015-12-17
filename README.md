SugarCRM CodeSniffer
====================
### Install PHP CodeSniffer

 * Linux:
```bash
pear install PHP_CodeSniffer
```

 * On Windows:
```bash
cd C:\xampp\php
php go-pear.phar
pear install PHP_CodeSniffer
pear upgrade
```

### Clone SugarCRM CodeSniffer

 * Linux:
```
git clone git@github.com:svnvcristea/SugarCRMCodeSniffer.git
```

 * Windows:
```
git clone https://github.com/svnvcristea/SugarCRMCodeSniffer.git
```

### Add SugarCS to the Standards

You have to copy the entire sub-folder SugarCS of this repo into the CodeSniffers Standards

 * Linux:
```bash
cd ./SugarCRMCodeSniffer
cp -r ./SugarCS   /usr/share/php/PHP/CodeSniffer/Standards/
```

 * Windows:
    Copy folder SugarCS to  ```C:\xampp\php\pear\PHP\CodeSniffer\Standards```

### Add SugarCS to PHPStorm Inspections Profile
* in PHPStorm from *File/Settings/Editor/Inspections*
* on the same line with the Profile, click Manage/Import , select SugarCRM_Default.xml
* from the Profile now select *SugarCRM Default*

This will Runs PHP Code Sniffer to find coding style problems based on SugarCS standards

### Make sure your PHPStorm is full configured

In PHPStorm from:

* in *File/Settings/Languages & Frameworks/PHP* set your PHP *Interpreter*
* in *File/Settings/Languages & Frameworks/PHP/CodeSniffer* from Configuration select or set your phpcs path:
    * Linux: ```/usr/bin/phpcs```
    * Windows: ```C:\xampp\php\phpcs.bat```


### Read more

SugarCS it's a standard based on PSR-2 with few exceptions. Read more about PSR-2 Coding Standards at:

* [PSR-2 Coding Style Guide](http://www.php-fig.org/psr/psr-2/)
* [Git pre-commit hook adjusted for SugarCRM CodeSniffer.](https://github.com/d-pluschaev/CsPCHookSugar)


### Have a look over:

* [sugarBash helper](https://github.com/svnvcristea/sugarBash)