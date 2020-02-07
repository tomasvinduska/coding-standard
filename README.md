## Coding standard

### Installing
```
composer require --dev tomasvinduska/coding-standard
```

additionaly you can add this to simplify commands calling

```json
"scripts": {
    "syntax": "vendor/bin/parallel-lint --exclude vendor .",
    "coding": "./vendor/bin/phpcs --standard=vendor/tomasvinduska/coding-standard/src/ruleset.xml --report=summary --ignore=vendor/*,temp/* --extensions=php --tab-width=4 -sp .",
    "coding-fix": "./vendor/bin/phpcbf --standard=vendor/tomasvinduska/coding-standard/src/ruleset.xml --ignore=vendor/*,temp/* --extensions=php --tab-width=4 -p ."
  }
```

