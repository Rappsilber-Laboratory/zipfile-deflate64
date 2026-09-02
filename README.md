# xicommon-zipfile-deflate64
[![PyPI](https://img.shields.io/pypi/v/xicommon-zipfile-deflate64)](https://pypi.org/project/xicommon-zipfile-deflate64/)

**WARNING:**
This package is a fork of zipfile-deflate64 and is only intended for usage in the [Rappsilber-Laboratory/xicommon](https://github.com/Rappsilber-Laboratory/xicommon) project. It will not be maintained for any other purposes.
The main objective of this fork is to support free threaded Python.

Extract Deflate64 ZIP archives with Python's `zipfile` API.

## Installation
```bash
pip install xicommon-zipfile-deflate64
```


## Usage
Anywhere in a Python codebase:
```python
import zipfile_deflate64  # This has the side effect of patching the zipfile module to support Deflate64
```

Alternatively, `zipfile_deflate64` re-exports the `zipfile` API, as a convenience:
```python
import zipfile_deflate64 as zipfile

zipfile.ZipFile(...)
...
```


