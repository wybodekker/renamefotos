# renamefotos
|     key | description
|     ---:|:---
|  script | renamefotos - rename all image/movie files in current dir
|    type | bash
|  author | Wybo Dekker
|   email | wybo@dekkerdocumenten.nl
| version | 1.01
| license | GNU General Public License

renamefotos renames all .jpg, .jpeg, .mov, .asf, .mts, and .avi
files in the current directory, using the creation date as reported by
exiftool, using its -createdate, -gpsdatetime, and -datetimeoriginal
options, in that order.
No file is renamed if any of the files does not contain a date, as that
would change file order. Upper case extensions are converted to lower case,
jpeg is converted to jpg.
