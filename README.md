# utils

Collection of simple utilities for (my) daily tasks

## List of utilities

- [cvc](https://raw.githubusercontent.com/nxnev/utils/master/bin/cvc)
  - Description: Comfy video converter
  - Usage:
    - Add videos of `dir` to batch script: `cvc /path/to/dir`
    - Start batch script: `cvc e`
- [cbz](https://raw.githubusercontent.com/nxnev/utils/master/bin/cbz)
  - Description: Create CBZs
  - Usage: `cbz /path/to/dir` (file will be saved as `/path/to/dir.cbz`)
- [mal-add](https://raw.githubusercontent.com/nxnev/utils/master/bin/mal-add)
  - Description: Add every anime listed on MyAnimeList into your list
  - Usage: `mal-add page` (where `page` refers to a certain number of page in [Just Added section](https://myanimelist.net/anime.php?o=9&c%5B0%5D=a&c%5B1%5D=d&cv=2&w=1).)
  - Example: `mal-add 12` (this would add every anime listed [here](https://myanimelist.net/anime.php?o=9&c[0]=a&c[1]=d&cv=2&w=1&show=550))
  - Notes:
    - This script doesn't work out of the box. Open it with some text editor and provide your `MALSESSIONID` cookie and the `csrf_token`.
    - It's possible to extend its functioning with another scripts. I'll add some later.
- [md5-renamer](https://raw.githubusercontent.com/nxnev/utils/master/bin/md5-renamer)
  - Description: Rename all files of current working directory as `{md5}.{ext}`
  - Usage: `md5-renamer`
- [ransg](https://raw.githubusercontent.com/nxnev/utils/master/bin/ransg)
  - Description: Random string generator
  - Usage: `ransg mode length amount`
    - `mode`: possible values are:
      - `1`: `a-z`
      - `2`: `a-z`, `A-Z`
      - `3`: `a-z`, `A-Z`, `0-9`
      - `4`: `a-z`, `A-Z`, `0-9`, ``!"#$%&'( )*+,-./:;<=>?@[\]^_`{|}~``
  - Examples:
    - ```
      $ ransg 2 12 4
      VfFPKHbEvUVN
      RaYWPApENYQe
      bdqCZKfvxZPe
      vyPrEUiVVuqY
      ```
    - ```
      $ ransg 4 64 2
      u-0?SzXR6?I~&K!bq#>D"FwPKn}h$TFrfu<AoZ)~.3v3s(ZbN^Dt9U#YbGP/}a<{
      X=1i]C4."DNWdOQPwu&(kkFZ~x2^.%.rHt!:d`M^mx)S{~+{X/^S']5h.7Pxl-L}
      ```
