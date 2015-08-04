This script uses PDO for the database connection.

In the example the actual HTML login form uses random sha1 keys that are valid once per load for the HTML input text login parts, making it impossible for bots/brute forcer's to differentiate between username and password form keys.

Passwords are hashed with sha512 @ 25k times with a 16byte user individual key salt.
Both hash and salt updates on successful login.
Brute force protection based on time interval between login attempts.


The source can be found here: https://code.google.com/p/php-pdo-secure-login-script-example/source/browse/branches/index.php