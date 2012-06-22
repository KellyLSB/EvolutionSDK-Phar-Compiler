EvolutionSDK Phar Compiler
==========================
This compiler is one of the easiest ways to get your [EvolutionSDK](http://github.com/EvolutionSDK/EvolutionSDK) (E3) site started. Not only do we compile the framework for you but we also have the ability to kick start your E3 site, but we also this will also keep your framework updated.

Dependencies
============
Ability to compile Phar files. The php.ini value `phar.readonly` must be set to '0'! This must be set in the php.ini file. You cannot set this with ini_set();

Ability to run PHP files from the Command Line.

Mac/*NIX System or server to run the script on.

Basic Usage
===========
To compile the framework go ahead and run `./compile`. This will automatically clone the repository and start the phar compilation process. The compiled Phar will now be accessible in the ./build directory.

Kickstart My Website
====================
To kick start your website with E3 run `./compile /path/to/site/dir`. This will clone and compile the phar just as if you had run `./compile`. It will also create the basic site structure to kick start your E3 site in the directory passed as the second argument. It will automatically copy the framework to the proper location and set up all the files. In fact all you need to do is set up apache to point to `/path/to/site/dir`.

EvolutionSDK comes with a built in management center to handle basic items, such as showing phpinfo() to setting environment variables. When you kickstart your E3 site with this script it will automatically ask you to set up your first development account.

Updating My E3 Framework
========================
This will only update the framework if you installed your framework using this compiler (or have your files in the exact same structure). All you need to run is `./compile /path/to/site/dir` it will replace the framework phar automatically.

Compiling a different branch of E3
==================================
You can compile an alternate branch of E3 by passing the branch name as the third argument (ie. `./compile /path/to/site/dir <branch>`). If all you want to do is compile the framework you can run `./compile false <branch>`

More by KellyLSB
================
Visit [KellyBecker.me](http://kellybecker.me)