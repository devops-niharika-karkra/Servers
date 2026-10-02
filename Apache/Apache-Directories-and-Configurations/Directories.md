# Apache directories 
Apache contains various directories each having its own specific function to perform.

## List of various directories with its purpose.
| Purpose | Directory |
|---------|-----------|
|Apache configuration|	/etc/apache2/|
|Main config	|/etc/apache2/apache2.conf|
|Virtual hosts	|/etc/apache2/sites-available/|
|Enabled virtual hosts	|/etc/apache2/sites-enabled/|
|Apache modules	|/etc/apache2/mods-available/|
|Enabled modules	|/etc/apache2/mods-enabled/|
|Document root|	/var/www/html/|
|Logs|	/var/log/apache2/|
|Runtime| files	/var/run/apache2/ or /run/apache2/|

## Apache configuration
``/etc/apache2/``: The primary directory containing all global configuration files, subdirectories, and directives for the Apache web server.

## Main config
``/etc/apache2/apache2.conf``: The central configuration file that defines global server behavior, default limits, and includes all other sub-configurations.

## Virtual hosts
``/etc/apache2/sites-available/``: Holds configuration files for all potential website domain setups (virtual hosts), whether they are currently active or not.

## Enabled virtual hosts
``/etc/apache2/sites-enabled/``: Contains symbolic links pointing to the configurations in sites-available/ that are currently active and served by Apache.

## Available modules
``/etc/apache2/mods-available/``: Stores configuration and load files for all Apache modules installed on the system, regardless of activation state.

## Enabled modules
``/etc/apache2/mods-enabled/``: Holds symbolic links to the modules in mods-available/ that are actively loaded into the web server.

## Document root
``/var/www/html/``: The default root folder where static website files, scripts, and web media served to site visitors are stored.

## Logs
``/var/log/apache2/``: Stores all server log files, including access.log for HTTP requests and error.log for troubleshooting system failures.

## Runtime files
``/var/run/apache2/`` or ``/run/apache2/``: Contains volatile runtime data, such as process IDs (PIDs) and lock files, required while Apache is actively executing.
