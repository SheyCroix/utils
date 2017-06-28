# utils

Collection of simple utilities for (my) daily tasks

## List of utilities

### [cbz](https://raw.githubusercontent.com/nxnev/utils/master/bin/cbz)
- Description: Create CBZs
- Usage: `cbz /path/to/dir` (file will be saved as `/path/to/dir.cbz`)

### [cvc](https://raw.githubusercontent.com/nxnev/utils/master/bin/cvc)
- Description: Comfy video converter
- Usage:
  - Add videos of `dir` to batch script: `cvc <dir1> <dir2> <dir3> ...`
  - Create new batch script: `cvc n`
  - Start batch script: `cvc s`

### [mal-add](https://raw.githubusercontent.com/nxnev/utils/master/bin/mal-add)
- Description: Add every anime listed on MyAnimeList into your list
- Usage: `mal-add page` (where `page` refers to a certain number of page in [Just Added section](https://myanimelist.net/anime.php?o=9&c%5B0%5D=a&c%5B1%5D=d&cv=2&w=1).)
- Example: `mal-add 12` (this would add every anime listed [here](https://myanimelist.net/anime.php?o=9&c[0]=a&c[1]=d&cv=2&w=1&show=550))
- Notes:
  - This script doesn't work out of the box. Open it with some text editor and provide your `MALSESSIONID` cookie and the `csrf_token`.
  - It's possible to extend its functioning with another scripts, like `mal-batch`.

### [mal-batch](https://raw.githubusercontent.com/nxnev/utils/master/bin/mal-batch)
- Usage: `mal-batch start end`

### [mal-comment](https://raw.githubusercontent.com/nxnev/utils/master/bin/mal-comment)
- Usage:
  - Get a list of users of certain club: `mal-comment e <club-id> <page-a> <page-b> [<output-file>]`
  - Post comment: `mal-comment c <users-list> <comment-file> [<logfile>]`
- Examples:
  - Get a list of all users of [graph.anime.plus](https://myanimelist.net/clubs.php?cid=67199)' club: `mal-comment e 67199 1 184 ~/graph-anime-plus.txt`
  - Deliver newsletter to all users of [graph.anime.plus](https://myanimelist.net/clubs.php?cid=67199)\' club: `mal-comment c ~/graph-anime-plus.txt ~/newsletter.txt ~/log.txt`
- Notes:
  - This script doesn't work out of the box. Open it with some text editor and provide your `MALSESSIONID` cookie and the `csrf_token`.
  - You can set variable `v_check` with some string to avoid duplicated comments when running the script multiple times using the same `<users-list>` file.

### [md5-renamer](https://raw.githubusercontent.com/nxnev/utils/master/bin/md5-renamer)
- Description: Rename all files of `dir` as `{md5}.{ext}`
- Usage: `md5-renamer <dir1> <dir2> <dir3> ...`

### [ransg](https://raw.githubusercontent.com/nxnev/utils/master/bin/ransg)
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
    X=1i]C4."DNWdOQPwu&(kkFZ~x2^.%.rHt!:d_M^mx)S{~+{X/^S']5h.7Pxl-L}
    ```
### [sadpanda](https://raw.githubusercontent.com/nxnev/utils/master/bin/sadpanda)
- Description: ExHentai Gallery Downloader
- Usage: `sadpanda <url> <start> <end> [<output-directory>]`
- Examples:
  - `sadpanda https://exhentai.org/g/1063613/4c498bd710/ 1 64` (this would download all pictures of [this gallery](https://exhentai.org/g/1063613/4c498bd710) in current directory)
  - `sadpanda https://exhentai.org/g/353151/00a898bae1 74 78 ~/Pictures/Saya` (this would download from page 74 to page 78 of [this gallery](https://exhentai.org/g/353151/00a898bae1) in ~/Pictures/Saya)
- Notes:
  - This script doesn't work out of the box. Open it with some text editor and provide your `ipb_member_id` and `ipb_pass_hash` cookies

### [tmo](https://raw.githubusercontent.com/nxnev/utils/master/bin/tmo)
- Description: TuMangaOnline Downloader
- Usage: `tmo <url>`
- Notes:
  - Images will be saved in your current directory.
