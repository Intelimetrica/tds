# v0.2.0-dev
* Bug Fixes
  * Fixed issue with empty strings and binaries being converted to nil

* Enhancements
  * datetime2 with 0 usec's will be transmitted as datetime

* Backwards incompatable changes
  * Changed datetime to be passed back as {{year, month, day} ,{hour, min, sec, microsec}}

# v0.1.6
* Bug Fixes
  * Changed default connection timeout to 5000 from :infinity
  * Added caller pid monitoring to cancel query if caller dies
  * Call ATTN if the caller who dies is the currently executing query

* Enhancements
  * Added API for ATTN call

# v0.1.5
* Bug Fixes
  * Fixed issue where driver would not call Connection.next when setting the state to :ready
  * Fixed UCS2 Encoding

# v0.1.4
* Bug Fixes
  * Fixed encoding for integers

# v0.1.3
* Bug Fixes
  * Removed Timer from queued commands.
  * Changed error handling to error func

# v0.1.2
* Bug Fixes
  * Adding missing date time decoders
  * Compatibility updates for ecto

# v0.1.1
* Bug Fixes
  * Fixed issue with Bitn always returning true
  * Fixed missing data return for char data decoding
  * Added float encoders

* General
  * Cleaned up logger functions

# v0.1.0 (2015-02-02)
* First Release