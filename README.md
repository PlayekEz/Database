# Database
This project will start with the purpose of making a similar to Config.php to be able to handle SQLite3 and MySQL databases with the same functions

# How to use


To start an instance with the library, two parameters will be required

* $db = new Database(String $path, int $type = Database::SQL);

Simple functions 

* $db->setInt(String $key, int $value);
* $db->setString(String $key, String $value);

In the case of the array they are separated by points so if there is a point in your value to save it may be confused!

* $db->setArray(String $key, Array $values);

You can also create a table initially, no SQL knowledge required

* $db->createTable(String $tableName, Array $data);

* Example: $db->createTable("City", ["id" => "PRINCIPAL" => "name" => "STRING"]);
* Supported values: PRINCIPAL | INT | STRING | BOOLEAN

And to save the stored data the basic function will be used

* $db->save();

This will only be to test its operation, it may be subject to errors but it will be solved. Anyway, if you can report the error, I would appreciate it.
# This is focused on pocketmine software
To avoid confusion, this little library is focused on pocketmine software for novice developers.
