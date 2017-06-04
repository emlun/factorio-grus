# GRand Unified Storage system

*GRUS*, the *GRand Unified Storage system* is a collection of blueprints for
storing and retrieving arbitrary collections of items using no provider or
requester chests.

![Screenshot](images/grus.png)

The system consists of 3 main parts:

- An [expandable storage unit][driver], top right
- A [programmed loading station][loading-station], top left
- A [programmed unloading station][unloading-station], bottom


Example uses:

- Load trains with supplies consisting of many different kinds of items, and
  delivering those supplies to outposts as needed
- Store strip mined resources your factory cannot consume quickly enough

Importable blueprint book string available [here][book].


## Usage

The components can be used on their own in other designs, or together

See the individual component manuals for details on how to set each component
up.

 1. Set up a storage unit. A storage unit is one [GRUS storage driver][driver]
    connected to a chain of one or more [GRUS storage cells][cell].
 2. Connect resource input to the input belts of the storage unit. The [GRUS
    programmed unloading station][unloading-station] can be used for this, and
    it will also only unload approximately the item quantities configured in
    the storage driver request signal.
 3. Connect request signals and output belts to the storage driver as needed,
    for example to a [GRUS programmed loading station][loading-station] for
    loading trains with item counts configured per train.


## Author

Blueprint designs by by Emil "emlun" Lundberg. Licensed under [Creative Commons
Attribution-ShareAlike 4.0][cc].

[driver]: storage-driver.md
[cell]: storage-cell.md
[loading-station]: programmed-loading-station.md
[unloading-station]: programmed-unloading-station.md
[book]: blueprint-book.txt
[cc]: https://creativecommons.org/licenses/by-sa/4.0/
