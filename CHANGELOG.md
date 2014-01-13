# v0.3.1-dev

* Enhancements
  * Compact state before printing to logs and hide password
  * Concurrency support, safe to use connection from multiple processes concurrently

# v0.3.0 (2013-12-16)

* Bug fixes
  * Don't try to decode values of text format

* Backwards incompatible changes
  * Types are stored as binaries instead of atoms, update your custom encoders and decoders


# v0.2.1 (2013-12-10)

* Enhancements
  * Add support for SSL

* Bug fixes
  * Fix decoding of unknown type when using custom decoder


# v0.2.0 (2013-11-14)

* Enhancements
  * Floats handles NaN, inf and -inf
  * Add support for numerics
  * Custom encoders and decoders works on elements in arrays
  * Add support for composite types
  * Add functions that raise on error

* Bug fixes
  * INSERT query works with extended query parameters
  * Return proper `num_rows` on PostgreSQL 8.4
  * Fix race condition

* Backwards incompatible changes
  * Simplify custom decoding and encoding with default function