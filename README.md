# linux-curated-list-of-commands
Here I will put interesting commands which is used in daily basis.
The description of command line options will be provided in the next line in order.

## Archive
Gzipping a folder using pigz (parallel version of gzip):
`tar cv /path/to/source/directory | pigz -9 > /path/to/dest/file.tar.gz` 
`Create archive [c] | Verbose flag [v] | Highest compression ratio (-1 to -9)`



## Disk Management
How much space did files and folders of current directory consume?
`du -ah --max-depth=1 --exclude=./folder1 --exclude=./fil1` 
`Scan through all files [a] | Generate human readable consumed spaces [h] | Report only 1st lvl directory hierarchy [--max-depth] | Optionally exclude some directories [--exclude] 

