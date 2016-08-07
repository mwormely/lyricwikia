lyricwikia
==========

Python API to get song lyric from `LyricWikia`_

Usage
-----

You can use the ``lyrics`` command to look for a song lyrics.

    usage: lyrics [-h] [--separator SEPARATOR] ARTIST SONG

    Get lyrics of a song from LyricWikia

    positional arguments:
      ARTIST                Artist name
      SONG                  Song title

    optional arguments:
      -h, --help            show this help message and exit
      --separator SEPARATOR line separator


Example
-------

.. code::

    $ lyrics 'Led Zeppelin' 'Stairway to heaven'
    There's a lady who's sure all that glitters is gold
    ...


API
---

At the moment ``lyricwikia`` is composed by a single API (the one that is not
officially already provided by the official APIs): ``get_lyrics``.

.. code:: python

    import lyricwikia
    lyrics = lyricwikia.get_lyrics('Led Zeppelin', 'Stairway to heaven')


.. _LyricWikia: http://lyrics.wikia.com/