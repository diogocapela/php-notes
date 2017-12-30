# php-notes

### Regular Arrays
```php
$myList = array(23,400,12,'foo','21','<h1>Hello</h1>');

print_r($myList);

echo $myList[0]
```

### Associative Arrays
```php
$myList = array('first_name' => 'John', 'second_name' => 'Doe');

print_r($myList);

echo $myList['first_name']
```

### Concatenate
```php
$hello = 'Hello';
$world = 'World';

$combine = $hello . ' ' . $world;
```

### Single VS Double Quotes
```php
$color = red;

echo "I love $color"; // outputs -> I love red
echo 'I love $color'; // outputs -> I love $color
```

### Constants
```php
define("CONSTANT", "Hello world.");
echo CONSTANT; // outputs "Hello world."
echo Constant; // outputs "Constant" and issues a notice.

define("GREETING", "Hello you.", true);
echo GREETING; // outputs "Hello you."
echo Greeting; // outputs "Hello you."

// Works as of PHP 7
define('ANIMALS', array(
    'dog',
    'cat',
    'bird'
));
echo ANIMALS[1]; // outputs "cat"
```

### String Casing
```php
$myString = 'hello World, this is a big line of text';

// Uppercase first
echo ucfirst($myString); // Hello World, this is a big line of text

// Uppercase words
echo ucwords($myString); // Hello World, This Is A Big Line Of Text

// Lowercase all
echo strtolower($myString); // hello world, this is a big line of text

// Uppercase all
echo strtoupper($myString); // HELLO WORLD, THIS IS A BIG LINE OF TEXT
```

### String Handling
```php
$myString = 'hello World, this is a big line of text';

// Repeat
str_repeat($myString, 3);

// Make substring from one point to another
substr($myString, 4, 6);

// Find position of any specific word
strpos($myString, 'big');

// Find character
strchr($myString, 'W');

// Total length of string
strlen($myString);

// Trim string
trim(' one string between spaces ');

// Find specific word and show after
strstr($myString, 'this');

// Replace words with a new one
str_replace('World', 'Universe', $myString);
```
