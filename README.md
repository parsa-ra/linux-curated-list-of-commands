# linux-curated-list-of-commands
Here I will put interesting commands which is used in daily basis.
The description of command line options will be provided in the next line in order.

## Archive
Gzipping a folder using pigz (parallel version of gzip):     
`tar cv /path/to/source/directory | pigz -9 > /path/to/dest/file.tar.gz`     
`Create archive [c] | Verbose flag [v] | Highest compression ratio (-1 to -9)`    



## Disk Management
How much space did files and folders of current directory consume?   
`du -ah --max-depth=1 --exclude=./folder1 --exclude=./file1`    
`Scan through all files [a] | Generate consumed spaces in human readable format[h] | Report only 1st lvl directory hierarchy [--max-depth] | Optionally exclude some directories [--exclude]`    


## Multimedia
Displaying available information of media files using ffprobe(part of ffmpeg project).     
`ffprobe -v error -show-streams`     
`Setting log level [v] | Flag to force ffprobe to show metadata of all streams [show-streams]`     


