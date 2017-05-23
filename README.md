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
