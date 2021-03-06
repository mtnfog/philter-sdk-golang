# Philter SDK for Golang

The **Philter SDK for Golang** enables Go developers to easily work with Philter. [Philter](https://www.mtnfog.com/products/philter/) identifies and manipulates sensitive information like Protected Health Information (PHI) and personally identifiable information (PII) from natural language text.

Refer to [Philter API](https://philter.mtnfog.com/api/) documentation for details on the methods available.

[![Build Status](https://travis-ci.org/mtnfog/philter-sdk-golang.svg?branch=master)](https://travis-ci.org/mtnfog/philter-sdk-golang)

## Installation

`go get github.com/mtnfog/philter-sdk-golang/philter`

## Example Usage

With an available running instance of Philter, to filter text:

To filter text:

```
filterResponse := Filter("http://localhost:8080", "His SSN was 123-45-6789.", "context", "docid", "default", "token")
```

To filter with explanation:

```
explainResponse := Explain("http://localhost:8080", "His SSN was 123-45-6789.", "context", "docid", "default", "token")
```

## Release History

* 1.1.0 - Adds authentication support.
* 1.0.0 - Initial release.

## License

This project is licensed under the Apache License, version 2.0.

Copyright 2020 Mountain Fog, Inc.
Philter is a registered trademark of Mountain Fog, Inc.
