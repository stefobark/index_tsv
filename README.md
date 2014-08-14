####Indexing TSV files is easy!####
```test.tsv``` is nothing special. Just three lines I made up to show some of the different kinds of datatypes you can put into a Sphinx index. It includes a UNIX timestamp attribute, a json attribute, a multi-valued attribute and a regular full-text field. Oh yeah! Don't forget the id. Sphinx needs a unique document identifier.

```test_tsv.conf``` is the configuration file I used to build this simple little index. Take a look to learn more.

And, go read [this blog post](http://sphinxsearch.com/blog/2014/08/14/easy-indexing-with-tsvpipe/) for more information.

