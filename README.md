# linux-curated-list-of-commands
Here I will put interesting commands which is used in daily basis.
The description of command line options will be provided in the next line in order.

## Archive
Gzipping a folder using pigz (parallel version of gzip):     
`tar cv /path/to/source/directory | pigz -9 > /path/to/dest/file.tar.gz`     
`Create archive [c] | Verbose flag [v] | Compression ratio (-1 to -9)`    

## Security
Encrypting a file using `gpg`
`gpg -c ./test.mp4`

Descrypting a file using `gpg`
`gpg -d ./test.mp4.gpg > ./test.mp4`

## Disk Management
How much space did files and folders of current directory consume?   
`du -ah --max-depth=1 --exclude=./folder1 --exclude=./file1`    
`Scan through all files [a] | Generate consumed spaces in human readable format[h] | Report only 1st lvl directory hierarchy [--max-depth] | Optionally exclude some directories [--exclude]`    


## Multimedia
Displaying available information of media files using ffprobe(part of ffmpeg project).     
`ffprobe -v error -show-streams`     
`Setting log level [v] | Flag to force ffprobe to show metadata of all streams [show-streams]`     

Encoding videos using vaapi hardware accelerated libraries
`ffmpeg -hwaccel vaapi -hwaccel_output_format vaapi -i /input/file.mp4 -c:v hevc_vaapi /output/file.mp4`

## File Transfer
Resumable rsync transfer over ssh     
`rsync -avhP -e ssh source:/path/to/file dest/path/to/file`         
`Depicting archive flag [a] | Verbose flag [v] | human readable sizes flag [h] | specifyig picked program in remote host to ssh (over ssh) [e]`     

## Misc 
Generate Random Strings
`tr -dc "A-Za-z0-9!#$%&'()*+,-./:;<=>?@[\]^_{|}~" </dev/urandom | head -c 64  ; echo`


