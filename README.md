TaggableBehavior
====================

Installation
------------

Download TaggableBehavior.php and put it somewhere.

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

Behavior creates two persistent tables:
* tags (id, category_id, name)
* tags_categories (id, name)

Tags are realted to tags categories. Relation field category_id is not required.

Add to schema.xml:

``` xml
<behavior name="taggable" />
```

Behavior will add several methods to the Model:

``` php
public function addTags($tags, $category_id = null, PropelPDO $con = null)
public function removeTags($tags, $category_id = null)
public function addTag(Tag $tag)
public function removeTag(Tag $tag)
```

*category_id* is optional parameter.

Requirements
------------

Credits
-------
* https://bitbucket.org/glorpen/taggablebehaviorbundle
* https://github.com/vbardales/PropelTaggableBehaviorBundle

