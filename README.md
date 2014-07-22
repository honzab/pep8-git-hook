pep8-git-hook
=============

This commit hook goes through all lines that you're changing with your commit
and checks them for PEP-8 violations. It does not allow you to commit if you
have any violations in your changes.

The hook ignores all lines that are not changed by your changeset.

## Requirements

* ```pip install pep8```

## Known issues 

* As pep8 goes through the files on filesystem and not through the diff to
  look for the violations, you can trick it by fixing the violation but not
  actually staging it.

