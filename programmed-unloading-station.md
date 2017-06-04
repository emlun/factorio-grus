# GRUS component: Programmed unloading station

This is a component of the [GRand Unified Storage system][grus]: a train station
that unloads trains based on a signal specifying what quantities of what item to
unload.

![Screenshot](images/programmed-unloading-station-v1.png)

- Blueprint version: 1
- Factorio version: 0.15.x

## Usage

The circuit near the train stop compute what items to unload. The _request
signal_ on the green wire of the substation specifies what quantities of items
should be unloaded. The station will unload these items for as long as the train
contains them and the station's buffer chests contain less than the requested
amount.

The [GRUS storage driver][driver] and [GRUS programmed loading
station][loading-station] can send this kind of request signal.


## Blueprint string

Available in the [blueprint book][book].


## Author

Blueprint design by by Emil "emlun" Lundberg. Licensed under [Creative Commons
Attribution-ShareAlike 4.0][cc].

[grus]: https://github.com/emlun/factorio-grus/
[driver]: storage-driver.md
[loading-station]: programmed-loading-station.md
[book]: blueprint-book.txt
[cc]: https://creativecommons.org/licenses/by-sa/4.0/
