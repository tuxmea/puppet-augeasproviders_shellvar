# Reference

<!-- DO NOT EDIT: This document was generated by Puppet Strings -->

## Table of Contents

### Resource types

* [`shellvar`](#shellvar): Manages variables in simple shell scripts.

## Resource types

### <a name="shellvar"></a>`shellvar`

Manages variables in simple shell scripts.

#### Properties

The following properties are available in the `shellvar` type.

##### `comment`

Text to be stored in a comment immediately above the entry.
It will be automatically prepended with the name of the variable in order
for the provider to know whether it controls the comment or not.

##### `ensure`

Valid values: `present`, `absent`, `unset`, `exported`

Create or remove the shellvar entry

Default value: `present`

##### `value`

Value to change the variable to.

#### Parameters

The following parameters are available in the `shellvar` type.

* [`array_append`](#array_append)
* [`array_type`](#array_type)
* [`name`](#name)
* [`provider`](#provider)
* [`quoted`](#quoted)
* [`target`](#target)
* [`uncomment`](#uncomment)
* [`variable`](#variable)

##### <a name="array_append"></a>`array_append`

Valid values: ``false``, ``true``

Whether to add to existing array values or replace all values.

Default value: ``false``

##### <a name="array_type"></a>`array_type`

Valid values: `auto`, `string`, `array`

Type of array mapping to use, defaults to `auto`.

* `auto` will detect the current type, and default to `string`
* `string` will render the array as a string and use space-separated values
* `array` will render the array as a shell array

Default value: `auto`

##### <a name="name"></a>`name`

The default namevar

##### <a name="provider"></a>`provider`

The specific backend to use for this `shellvar` resource. You will seldom need to specify this --- Puppet will usually
discover the appropriate provider for your platform.

##### <a name="quoted"></a>`quoted`

Valid values: `auto`, `double`, `single`, `none`, ``false``, ``true``

Quoting method to use, defaults to `auto`.

* `auto` will quote only if necessary, leaving existing quotes as-is
* `double` and `single` will always quotes
* `none` will remove quotes, which may result in save failures

Default value: `auto`

##### <a name="target"></a>`target`

namevar

The file in which to store the variable.

##### <a name="uncomment"></a>`uncomment`

Valid values: ``true``, ``false``

Whether to remove commented value when found.

Default value: ``false``

##### <a name="variable"></a>`variable`

namevar

The name of the variable, e.g. OPTIONS

