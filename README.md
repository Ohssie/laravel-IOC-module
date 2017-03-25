#Laravel-IOC-Module
Laravel made available the IoC[Inversion of Control] container for developers. This bash script is aimed at speeding up development for Laravel developers.

## How to use
Add the file to the root of your Laravel project directory and  run it like so: **./ioc.sh**.

In cases where you're going to use it on an online development environment, you need to assign permission to make the script executable like so: **chmod +x ioc.sh**

## What it does
After running the bash script, you will be prompted for a module name. After that input, the following is performed as a result of that:
- A Laravel model is created in the **app** directory.
- A migration file is created with the module name in **database/migrations**.
- A Service provider is created in **app/Providers** and registered inside **config/app.php** under the **providers** section.
- A Laravel Controller is created for you in **app/Http/Controllers** which implements all CRUD methods with necessary Dependency Injections.
- A Repositories directory which houses your repository files is created in the **app** directory.
- A Repository and Contract file is created inside **app/Repositories/module_name** directory.
- Your repository and contract files are bound inside the respective Service Providers.
- Three view files are created inside the **resources/views/module_name** directory and they are: **index.blade.php**, **create.blade.php** and **edit.blade.php**.

## Contributors
[Eric Renouf](http://stackoverflow.com/users/4687135/eric-renouf/) on [Stackoverflow](http://stackoverflow.com/)

> *Made with love from [nHub Nigeria](http://nhubnigeria.com/)*
