Coding Guideline for PHP
========================

Installation
------------

You have to require the package via composer `composer require codappix/cgl-php`.
After that you have to add the following to the `composer.json`:

    "scripts": {
        "post-autoload-dump": [
            "[ -d vendor/squizlabs/php_codesniffer/CodeSniffer/Standards/CGL-PHP ] || cp -r vendor/codappix/cgl-php vendor/squizlabs/php_codesniffer/CodeSniffer/Standards/CGL-PHP"
        ]
    }

What does it do?
----------------

The goal of this package is to provide our PHP cgl rules, which are based on PSR-2, via composer.
The package uses PHP_CodeSniffer to sniff the configured PHP files and show errors.

Current state
-------------

This is the initial version of this ruleset. We are currently only using the PSR-2 rules.
Custom rules and sniffs will follow when needed.

This is a early version. More information can be taken from Github at
`current issues`_.

.. _current issues: https://github.com/Codappix/CGL-PHP/issues
