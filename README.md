By default, json_encode() converts UTF-8 characters to Unicode escape sequences while serialize() does not. Note: To leave UTF-8 characters untouched, you can use the option JSON_UNESCAPED_UNICODE as of PHP 5.4.

JSON will have no memory of what the object's original class was (they are always restored as instances of stdClass).
