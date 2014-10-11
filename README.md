JSON_Encode-VS-PHP_Serialize
============================

A simple speed test to compare json_encode() and serialize()

Some difference between json_encode() and serialize():

- By default, json_encode() converts UTF-8 characters to Unicode escape sequences while serialize() does not.
Note: To leave UTF-8 characters untouched, you can use the option JSON_UNESCAPED_UNICODE as of PHP 5.4.

- JSON will have no memory of what the object's original class was (they are always restored as instances of stdClass).

- You can't leverage __sleep() and __wakeup() with JSON

- Only public properties are serialized with JSON

- JSON is more portable
