# project path
!-- keep the format -->
## Start Date of project

```bash <!-- markdownlint-disable-line code-block-style -->
$ date
Fri Jul 25 09:07:19 AM CEST 2025
```

## Environment

### Os
<!-- keep the format -->
```bash
uname -a
Linux debian 6.1.0-37-amd64 #1 SMP PREEMPT_DYNAMIC Debian 6.1.140-1 (2025-05-22) x86_64 GNU/Linux
```

## Point release
<!-- keep the format -->
```bash
cat /etc/debian_version
12.11
```
<!-- keep the format -->
## BASH version used
<!-- keep the format -->
```bash
echo $BASH_VERSION
5.2.15(1)-release
```
<!-- keep the format -->
<!-- keep the format -->
>[!NOTE]
>Symbol to mark web external links [![alt text][1]](./README.md)
<!-- -->
>[!TIP]
>Get the link symbol with the curl command using the console
>
>>-m, --mode=MODE [![alt text][1]](https://www.man7.org/linux/man-pages/man1/mkdir.1.html) \
    set file mode (as in chmod), not a=rwx - umask
>><!-- -->
>>-p, --parents [![alt text][1]](https://www.man7.org/linux/man-pages/man1/mkdir.1.html) \
    no error if existing, make parent directories as needed,
    with their file modes unaffected by any -m option
><!-- -->
>```bash
># First make sure that the target directory exists
>mkdir -p ./img &&
>curl --create-dirs --output-dir img -O  "https://raw.githubusercontent.com/MathiasStadler/link_symbol_svg/360d1327d05280d53de5fa816c522f89a35891ca/img/link_symbol.svg"
>```
<!-- keep the format -->
>[!TIP]
>Add the reference of the link image at the end of the Markdown file
<!-- keep the format -->
>```bash
># project_path.md
># printf "<\041\055\055" >> ./project_path.md
>printf "<\041\055\055 Link sign - Don't Found a better way :-( - You know a better method? - send me a email -->\n[1]: ./img/link_symbol.svg\n"  >> ./project_path.md
>#README.md
> printf "<\041\055\055 Link sign - Don't Found a better way :-( - You know a better method? - send me a email -->\n [1]: ./img/link_symbol.svg\n"  >> ./README.md
>```
<!-- keep the format -->
>[!TIP]
>How to redirect a output of a command to two files [![alt text][1]](https://stackoverflow.com/questions/625571/how-to-redirect-a-output-of-a-command-to-two-files)  
>```date | tee file1 >> file2```
<!-- keep the format -->
>[!TIP]
>Avoid markdownlint error MD053 - Link and image reference definitions should be needed
<!-- keep the format -->
>```bash
>> printf "<\041\055\055 Avoid markdownlint error MD053 - Link and image reference definitions should be needed-->" tee ./README.md >> ./project_path.md
>> printf "- Link of this file [![alt text][1]](./README.md)" tee ./README.md >> ./project_path.md
>># online
>> printf "<\041\055\055 Avoid markdownlint error MD053 - Link and image reference definitions should be needed--> \n- Link of this file [![alt text][1]](./README.md)" tee ./README.md >> ./project_path.md
>```
<!-- keep the format -->
<!-- Link sign - Don't Found a better way :-( - You know a better method? - send me a email -->
[1]: ./img/link_symbol.svg
