# PHP

We are mainly using psr-2(http://www.php-fig.org/psr/psr-2/) as our coding standard but we are not using all of its standards that we do not agree on.

## Indents

Unlike psr-2 we are using tab indents over spaces for line beginnings.

We use tab size of 4.

```php
<?php
if (...)
{
  $var = 1;
}
?>
```

The only exception for this is when aligning arrays, that will be done via spaces otherwise it causes alignment issues on linux and other formatters.

```php
<?php
$array = [
  'name'    => 'test',
  'surname' => 'test2',
];
?>
```

## Arrays

We use square bracket arrays as psr-2 uses, note that this will not support anything lower than php 5.4 as to push forward the requirements.

```php
<?php
$array = [];
?>
```

## Namespace & Use

Namespaces should be on the first line directly after the php open tag.

```php
<?php namespace Foo\Bar;

?>
```

Each use should have its own line, *except* for aliases which can share a use statement.

Aliases should appear before other use statements.

```php
<?php
use Config, File;
use Foo\Bar;
use Foo\Chart;
?>
```

## Curly Parentheses

Should be on a new line to better format how the code structure and indents are.

```php
<?php
class Name
{
  // code here
}
?>
```

```php
<?php
function test()
{
  // code here
}
?>
```

## Class functions

Prefix the function name with the request type.

```php
<?php namespace Foo\Bar;

class Bar
{
  public function getIndex()
  {
    // code
  }
  
  public function postIndex()
  {
    // code
  }
}
```