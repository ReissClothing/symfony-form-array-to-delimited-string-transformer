Array to delimited string data transformer
==========================================

This is a data transformer for the Symfony form framework.

It will transform a string input, such as `foo, bar, bar, foo` to an array
e.g. `array('foo', 'bar', bar', foo')`.

Usage
-----

````php
$form->add($builder->create('tags', 'text')->addModelTransformer(new ArrayToDelimitedStringTransformer()))
````
