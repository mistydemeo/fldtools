# fldtools

This tool supports unpacking and authoring FLD data files from the game [*Magical School Lunar!*](https://en.wikipedia.org/wiki/Lunar:_Samposuru_Gakuen) (Sega Saturn, 1997).

## Installation

On Mac:

> brew install mistydemeo/lunar/fldtools

Building manually:

Clone this repo, and then

> make

## Usage

### fldunpack

fldunpack FILENAME.FLD

The chunks will be extracted to a set of numbered files with filenames based on the filename from which they were extracted. By default, chunks will be extracted with the file extension "chunk"; use the `--extension` option to choose a custom file extension. This is useful when extracting data from the `MSLM.FLD` file, which contains FMVs, since other apps will expect a `.cpk` extension from its contents.

### fldpack

fldpack output.fld <input files>
