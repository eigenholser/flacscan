==============================
FLAC Scanner and MP3 Converter
==============================

I wrote this many years ago but then stopped listening to MP3 audio in favor of
straight FLAC which does sound better. Recently I took a renewed interest in
this utility, dusted it off and added APIC tagging for cover art. It may have
potential beyond MP3 conversion for those that might be pedantic about managing
their digital music library.

Scan FLAC directory. Compare each file with corresponding MP3 file. If there is
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

