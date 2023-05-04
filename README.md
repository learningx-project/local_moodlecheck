Moodle PHPdoc Checker
=====================

[![Moodlecheck CI](https://github.com/moodlehq/moodle-local_moodlecheck/actions/workflows/ci.yml/badge.svg)](https://github.com/moodlehq/moodle-local_moodlecheck/actions/workflows/ci.yml)

Installation:
-------------

Install the source into the local/moodlecheck directory in your moodle


To install it using git, type this command in the root of your Moodle install:

    git clone https://github.com/learningx-project/local_moodlecheck.git local/moodlecheck

Then add /local/moodlecheck to your git ignore.


After you have installed this local plugin, you
should Log in as admin and select:

> Site administration -> Development -> Moodle PHPdoc check

Enter paths to check and select rules to use.

Customization:
--------------

You can add new rules by adding new php files in rules/ directory,
they will be included automatically.

Look at other files in this directory for examples.

Please note that if you register the rule with code 'mynewrule',
the rule registry will look in language file for strings
'rule_mynewrule' and 'error_mynewrule'. If they are not present,
the rule code will be used instead of the rule name and
default error message appears.
