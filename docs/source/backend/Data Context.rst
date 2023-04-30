Data Context
============

The ``DataContext`` class (located in the ``backend_dotnet\Data\DataContext.cs`` file) is responsible for managing the connection to the database and providing access to the various tables within the database. This class inherits from the ``DbContext`` class provided by the Entity Framework Core library.

DataSets
--------

The following data sets are defined within the DataContext class:

- Projects: Represents the table containing project data.
- Users: Represents the table containing user data.
- ProjectPermissions: Represents the table containing project permissions data.
- Ratings: Represents the table containing ratings data.

Database Connection Configuration
---------------------------------

The ``OnConfiguring`` method in the DataContext class is used to configure the database connection. It retrieves the server, database, username, and password from environment variables, and configures the connection to use the MySQL database with the specified credentials.

Logging Configuration
---------------------

The DataContext class also configures logging for the database context. It uses the LoggerFactory to create a logging provider that outputs log messages to the console, with a log level filter set to "Warning" for messages coming from the "Microsoft.EntityFrameworkCore" namespace. Additionally, sensitive data logging and detailed error messages are enabled.
