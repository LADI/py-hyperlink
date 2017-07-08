# Hyperlink

*Cool URLs that don't change.*

<a href="https://hyperlink.readthedocs.io/en/latest/"><img src="https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat"></a>
<a href="https://pypi.python.org/pypi/hyperlink"><img src="https://img.shields.io/pypi/v/boltons.svg"></a>
<a href="http://calver.org"><img src="https://img.shields.io/badge/calver-YY.MINOR.MICRO-22bfda.svg"></a>

Hyperlink provides a pure-Python implementation of immutable
URLs. Based on [RFC 3986][rfc3986] and [3987][rfc3987], the Hyperlink URL
makes working with both URIs and IRIs easy.

Hyperlink is tested against Python 2.7, 3.4, 3.5, 3.6, and PyPy.

Full documentation is available on [Read the Docs][docs].

[rfc3986]: https://tools.ietf.org/html/rfc3986
[rfc3987]: https://tools.ietf.org/html/rfc3987
[docs]: http://hyperlink.readthedocs.io/en/latest/

## Installation

Hyperlink is a pure-Python package and requires nothing but
Python. The easiest way to install is with pip:

```
pip install hyperlink
```

Then, hyperlink away!

```python
from hyperlink import URL

url = URL.from_text('http://github.com/mahmoud/hyperlink?utm_source=README')
utm_source = url.get('utm_source')
better_url = url.replace(scheme='https')
user_url = better_url.click('..')
```

See the full API docs on [Read the Docs][docs].

## More information

Hyperlink would not have been possible without the help of
[Glyph Lefkowitz](https://glyph.twistedmatrix.com/) and many other
community members, especially considering that it started as an
extract from the Twisted networking library. Thanks to them,
Hyperlink's URL has been production-grade for well over a decade.

Still, should you encounter any issues, do file an issue, or submit a
pull request.
