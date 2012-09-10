LikeableBehavior
====================

Installation
------------

Download TaggavleBehavior.php and put it somewhere.

``` ini
propel.behavior.taggable.class = path.to.taggable.behavior
```

If you are using composer then just add:
```js
{
    "require": {
        "smirik/propel-taggable-behavior": "*"
    }
}
```

The ini-configuration would be
``` ini
propel.behavior.taggable.class = vendor.smirik.src.propel-taggable-behavior.src.TaggableBehavior
```

Usage
-----

Add to schema.xml:

``` xml
<behavior name="taggable" />
```

Behavior will create table *likes* and add several methods to the Model:

``` php

```

*user_id* could be any integer.

Requirements
------------

Credits
-------
* https://bitbucket.org/glorpen/taggablebehaviorbundle
* https://github.com/vbardales/PropelTaggableBehaviorBundle

