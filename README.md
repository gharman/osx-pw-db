osx-pw-db
=========

Command-line (encrypted) password database for OSX. The actual database file (i.e. for backup) is located at ~/.pwdb

All passwords are stored as key/value pairs where key is an arbitrary identifiers and value is the password. Note that in all cases, a "database password" is requested; this is used to encrypt the (value) password. 

Usage:

Add a new password: pw add <password>
Delete a password: pw delete <key>
Generate a password for a new key: pw gen <key>
Retrieve a password (to the copy/paste buffer): pw <key>
List all keys: pw list
List all keys starting with foo: pw list foo

Installation:

Copy the file pw to a location that is on your shell path. Ensure that it has executable permission (e.g. chmod 755 pw)
