# Netgen Layouts Relation List Query

This bundle provides Netgen Layouts query that makes it possible to add items to
block via relation list field type available in any content in eZ Platform CMS.

## Installation instructions

### Use Composer

Run the following from your installation root to install the package:

```bash
$ composer require netgen/layouts-relation-list-query:^1.0
```

### Activate the bundle in your app kernel

Add the following to the list of activated bundles:

```php
$bundles = [
...

new Netgen\Bundle\LayoutsRelationListQueryBundle\NetgenLayoutsRelationListQueryBundle(),

...
];
```

Due to how prepending configuration of other bundles works in Symfony, to make
this query type display after the existing eZ Platform query type, you need to
add the bundle BEFORE `NetgenLayoutsEzPlaformBundle` in the list of
activated bundles.
