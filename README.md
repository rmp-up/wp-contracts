# WordPress contracts

> Helper for PHP (especially WordPress)

## Features

* Rewindable Generators
* Hydrate and exchange protected fields in objects
* [System logger](https://php.net/syslog) compatible logging:
  * Forward to `syslog()`
  * Delegate to [PSR-3 logger](https://www.php-fig.org/psr/psr-3/)
  * Forward to [`error_log()`](https://php.net/function.error-log)
    respecting configured [error reporting levels](https://php.net/error_reporting)
  * Forward to [WP_CLI](https://make.wordpress.org/cli/)
  * Append to an [array-like variable/reference](https://www.php.net/class.arrayaccess)
* Message Bus (delegating to WP_Hook)
  * Decouple exception handling per action/filter
  * Stop propagation

Tested with:

* PHP 7.0 - 7.4
* WordPress >= 4.5
