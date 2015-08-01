broccoli-file-size
==================

[![Build Status](https://img.shields.io/travis/amercier/broccoli-file-size/master.svg)](https://travis-ci.org/amercier/broccoli-file-size)

Broccoli plugin to display file sizes. Example output:

    > broccoli build dist

    file1.txt => 446 kB (284 kB gzipped)
    file2.txt => 223 kB (74 kB gzipped)
    file3.txt => 543 kB (324 B gzipped)

Installation
============

    npm install --save-dev broccoli-file-size

Usage
=====

    var fileSize = require('broccoli-file-size');
    tree = fileSize(tree);

Options
=======

    tree = fileSize(tree, {
      colors: true,
      gzipped: true
    });

### colors

Enable/disable colors (default: `true`).

### gzipped

Show/hide gzipped size (default: `true`).
