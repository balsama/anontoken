#Anonymous Tokens

This module emulates the behavior of the `drupal_get_token()` and
`drupal_token_valid()` function in common.inc replacing the `session_id()`
variable with a unique per visitor ID generated by the UUUID module. This
allows you to use tokens with anonymous users the same way you can with
authenticated users.

###Function Equivalents

* `drupal_get_token($value = '')` becomes `anontoken_get($value = '')`
* `drupal_token_valid($token, $value = '')` becomes `anontoken_valid($token, $value = '')`

See the comments in the .module file for more information. This module is
dpendant on the Universally Unique User ID module (not to be confised with the
Universally Unique ID module).
