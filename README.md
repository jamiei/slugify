# Slugify

Simple slug generator. Transforms strings into URL slugs, removing non-alphanumeric characters and spaces. Optionally you can set the delimiter and maximum url size.

## Usage
Add to project.clj:

    [slugify "0.0.1"]

## Usage

    (use 'slugify.core)
    => nil
    (slugify "charlie brown")
    => "charlie-brown"
    (slugify "    Charlie Brown    ")
    => "charlie-brown"
    (slugify "charlie brown" "_")
    => "charlie_brown"
    (slugify "joão da silva")
    => "joao-da-silva"
    (slugify "excessively long string" "-" 15)
    => "excessively-lon"

## License

Copyright (C) 2012 FIXME

Distributed under the Eclipse Public License, the same as Clojure.
