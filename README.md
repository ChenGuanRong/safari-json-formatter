# JSON Formatter

A Safari extension which makes valid JSON documents human-readable.

### Before:
![Before][i1]
### After:
![After][i2]

## Installation
[Download the extension][1] and open it with Safari 5.

### Usage
Once installed, load any valid JSON document. [This project's most recent
commit][2] makes a good example.

#### Version History

### 1.1
* Added folding of arrays, objects and long strings
* Added setting for auto-folding of long strings (default: on)
* Added setting for "long string" threshold (default 512 bytes)
* Added a "toggle formatting" button to switch between formatted and original JSON
* Bug Fixes

#### Caveats
The extension aims to produce the same JSON string that's been loaded as input,
but because the original JSON has actually been parsed, some transformation may
occur. In other words, the formatted JSON will always be equivalent to the
original JSON, but in rare circumstances it may not match exactly. The only
known example of this is kind of discrepancy is between number formats -- if the
original JSON contains the numeric value 1e2, for example, the formatted JSON
will display the value 100.

[1]: http://github.com/rfletcher/safari-json-formatter/downloads
[2]: http://github.com/rfletcher/safari-json-formatter/commit/HEAD.json
[i1]: https://github.com/rfletcher/safari-json-formatter/raw/HEAD/etc/images/before.png
[i2]: https://github.com/rfletcher/safari-json-formatter/raw/HEAD/etc/images/after.png