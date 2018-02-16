# Listal Image Batch Downloader

Simple bot to download pictures from [listal](www.listal.com)

## Setup

You will need to have [NodeJS](nodejs.org) installed to use or develop this.

To install as a command line tool, install it globally using NPM.

```
npm install listal -g
```

To use this directly from source:

```
node listal.js <arguments>
```

## Usage

(The usage guide assumes you have installed it globally)

For example, if you want to download all images in listal from inception just type:

```bash
listal -u http://www.listal.com/movie/inception
```

If you want all the pictures from the director:

```bash
listal -u http://www.listal.com/christopher-nolan
```

Or if you are on the naughty side and want the pictures of diCaprio or Ellen Page try:

```bash
listal -u http://www.listal.com/leonardo-dicaprio
listal -u http://www.listal.com/ellen-page
```

All pictures are downloaded by default to `target` but you can change this with the `-o` option.

If you want to skip any images you have already downloaded add the `-s` option.

You can specify the pages to download using the `-p` option.

```bash
listal -u http://www.listal.com/leonardo-dicaprio -p 10
listal -u http://www.listal.com/leonardo-dicaprio -p 10-15
```

If you want to skip any images you have already downloaded add the `-s` option

You can set the number of concurrent pages to process using option `-c`. The default is `5`. If you have problems downloading try lowering the value.

## To Do List

* Better handling of the `-u` option, for example accept bad urls
* Better code in some areas.

