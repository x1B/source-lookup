# source-lookup

> Post-mortem analysis of minified JavaScript

When you observe a production problem without having deployed source-maps, you will only have access to source coordinates within the minified bundle (line, column).
Point this script to your source-map to find out the corresponding source location.


## Installation

You can install `source-lookup` globally:

```console
> npm install -g source-lookup
```


## Usage

Get the original position for bundle line 23, column 5:

```console
> source-lookup 23:5 path/to/bundle.js.map
Source file: path/to/my-source.js
Source position: 5:0
```
