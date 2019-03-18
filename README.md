# ci-parsedown #

----

This is a Code Igniter equivalent package of the PHP Markdown library called 'Parsedown', which can be found at https://github.com/erusev/parsedown 

### Installation ###

To install, download the Splint terminal tool at https://splint.cynobit.com/downloads/splint and run 



```bash
splint install francis94c/ci-parsedown

```

from the root of your Code Igniter distribution.

### Loading ###

From anywhere (Controller, Model, etc.)

```php
$this->load->splint("francis94c/ci-parsedown", "+Parsedown", null, "parsedown");
```

### Auto-Loading ###

```php
$autoload["splint"] = array("francis94c/ci-parsedown" => array("+Parsedown", null, "parsedown"));
```

### Usage ###

After loading

```php
$output = $this->parsedown->text("_Hello World_"); // Whole conversion

$output = $this->parsedown->line("_Hello world_"); // Inline conversion
```

