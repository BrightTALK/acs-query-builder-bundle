# Amazon Cloud Search Query Builder Bundle

## Description

This bundle integrates Amazon Cloud Search Query Builder into Symfony2

##Installation

Add to your composer.json:

```json
"require": {
    ...
    "brighttalk/acs-query-builder": "dev-master",
    "brighttalk/acs-query-builder-bundle": "dev-master"
}
```

### add the bundle to the AppKernel

``` php
<?php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new BrightTALK\Bundle\ACSQueryBuilderBundle\BrightTALKACSQueryBuilderBundle()
    );
}
```

The service id brighttalk_acs_query_builder.query_builder_factory is now available to be used, and will create a new query builder by calling the method createQueryBuilder()