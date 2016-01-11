==============================
FLAC Scanner and MP3 Converter
==============================

Scan flac directory. Compare each file with corresponding MP3 file. If there is
no corresponding MP3 file, create one from the FLAC file.

-------
Tagging
-------

Tags from FLAC files will be used to tag the new MP3 files. ``ID3v2`` is forced.
A file named ``cover.*`` if present in the source directory will be used to
create an APIC frame in the MP3 file. The APIC frame will be ``image/jpeg``.

------------
Dependencies
------------

- Audio::FLAC::Header
- MP3::Tag
- IO::Interactive
- DBI
- DBD::SQLite
- sqlite3 package
- lame
- sox

