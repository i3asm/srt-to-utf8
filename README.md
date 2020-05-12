# srt-to-utf8
convert .srt files with cp1256 encoding (most arabic subtitles use it. that's why it shows a weird characters
until you change the encoding type in the your video player options) to utf-8 encoding.

unfortunately it can't detect the encoding as it is a known problem with no easy solution (as my quick googling said).

but if you are lucky and the encoding is Windows-1256, then your problem is solved.



## how it works

it will move recursively throw the current folder searching for a .srt file.
and if there is one, it will make a 'converted/' folder. this folder will contain all your converted subtitles as a utf-8 encoded ones.

#### NOTE: this is a bit risky. using it in the home directory will run it through all your .srt files and try to re-encode them recursively

## FUTURE PLANS
- [ ] make it work with other file extensions like txt or vvt
- [ ] make it convert to other encodings
