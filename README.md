####Indexing TSV files is easy!####
```test.tsv``` is nothing special. Just three lines I made up to show some of the different kinds of datatypes you can put into a Sphinx index. It includes a UNIX timestamp attribute, a json attribute, a multi-valued attribute and a regular full-text field. Oh yeah! Don't forget the id. Sphinx needs a unique document identifier.

```test_tsv.conf``` is the configuration file I used to build this simple little index. Take a look to learn more.

#####DOCID#####
```docid.sh``` is one way to add docids to each line of your tsv file. It just reads each line from a file and prints an incrementing DOCID to each line (followed by a tab).

In my case, I wanted to play around with UFO sighting descriptions. I came across [this](http://www.infochimps.com/datasets/60000-documented-ufo-sightings-with-text-descriptions-and-metada) and wanted to play around with it using Sphinx. I saw no unique keys, so I added them with this little script. Check it out, just change the file name to match yours and then, from the appropriate directory, run it:
```
sudo bash docid.sh
```

Also, go read [this blog post](http://sphinxsearch.com/blog/2014/08/14/easy-indexing-with-tsvpipe/) for more information.

