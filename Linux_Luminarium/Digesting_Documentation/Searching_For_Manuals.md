# Searching for Manuals
This challenge asks use to invoke the `/challenge/challenge` command with the write argument whose document is in a crazy file name which we need to see using the man command and to find that manual name we need to see documentation of `man` using `man man`
```bash
hacker@man~searching-for-manuals:~$ man man
MAN(1)                   Manual pager utils                  MAN(1)

NAME
       man - an interface to the system reference manuals

SYNOPSIS
       man [man options] [[section] page ...] ...
       man -k [apropos options] regexp ...
       man -K [man options] [section] term ...
       man -f [whatis options] page ...
       man -l [man options] file ...
       man -w|-W [man options] page ...

DESCRIPTION
       man  is the system's manual pager.  Each page argument given
       to man is normally the name of a program, utility  or  func‐
       tion.   The  manual page associated with each of these argu‐
       ments is then found and displayed.  A section, if  provided,
       will  direct man to look only in that section of the manual.
       The default action is to search in all of the available sec‐
       tions  following  a pre-defined order (see DEFAULTS), and to
       show only the first page found, even if page exists in  sev‐
       eral sections.

       The table below shows the section numbers of the manual fol‐
       lowed by the types of pages they contain.

       1   Executable programs or shell commands
       2   System calls (functions provided by the kernel)
       3   Library calls (functions within program libraries)
       4   Special files (usually found in /dev)
       5   File formats and conventions, e.g. /etc/passwd
       6   Games
       7   Miscellaneous  (including  macro  packages  and  conven‐
           tions), e.g. man(7), groff(7)
       8   System administration commands (usually only for root)
       9   Kernel routines [Non standard]

       A manual page consists of several sections.

       Conventional  section names include NAME, SYNOPSIS, CONFIGU‐
       RATION, DESCRIPTION, OPTIONS, EXIT STATUS, RETURN VALUE, ER‐
       RORS,  ENVIRONMENT,  FILES,  VERSIONS, CONFORMING TO, NOTES,
       BUGS, EXAMPLE, AUTHORS, and SEE ALSO.

       The following conventions apply to the SYNOPSIS section  and
       can be used as a guide in other sections.

       bold text          type exactly as shown.
       italic text        replace with appropriate argument.
       [-abc]             any  or  all arguments within [ ] are op‐
                          tional.
       -a|-b              options delimited by | cannot be used to‐
                          gether.
       argument ...       argument is repeatable.
       [expression] ...   entire  expression within  [ ] is repeat‐
                          able.

       Exact rendering may vary depending  on  the  output  device.
       For instance, man will usually not be able to render italics
       when running in a terminal, and will  typically  use  under‐
       lined or coloured text instead.

       The  command  or  function  illustration  is  a pattern that
       should match all possible invocations.  In some cases it  is
       advisable  to illustrate several exclusive invocations as is
       shown in the SYNOPSIS section of this manual page.

EXAMPLES
       man ls
           Display the manual page for the item (program) ls.

       man man.7
           Display the manual page for macro package man from  sec‐
           tion  7.   (This  is  an  alternative spelling of "man 7
           man".)

       man 'man(7)'
           Display the manual page for macro package man from  sec‐
           tion 7.  (This is another alternative spelling of "man 7
           man".  It may be more convenient when copying and  past‐
           ing  cross-references  to  manual  pages.  Note that the
           parentheses must normally be quoted to protect them from
           the shell.)

       man -a intro
           Display,  in succession, all of the available intro man‐
           ual pages contained within the manual.  It  is  possible
           to quit between successive displays or skip any of them.

       man -t bash | lpr -Pps
           Format  the  manual page for bash into the default troff
           or groff format and pipe it to  the  printer  named  ps.
           The default output for groff is usually PostScript.  man
           --help should advise as to which processor is  bound  to
           the -t option.

       man -l -Tdvi ./foo.1x.gz > ./foo.1x.dvi
           This command will decompress and format the nroff source
           manual page ./foo.1x.gz into a device independent  (dvi)
           file.   The  redirection  is  necessary  as  the -T flag
           causes output to be directed to stdout  with  no  pager.
           The  output  could be viewed with a program such as xdvi
           or further processed into  PostScript  using  a  program
           such as dvips.

       man -k printf
           Search  the short descriptions and manual page names for
/challenge
Pattern not found
hacker@man~searching-for-manuals:~$ man man
MAN(1)                   Manual pager utils                  MAN(1)

NAME
       man - an interface to the system reference manuals

SYNOPSIS
       man [man options] [[section] page ...] ...
       man -k [apropos options] regexp ...
       man -K [man options] [section] term ...
       man -f [whatis options] page ...
       man -l [man options] file ...
       man -w|-W [man options] page ...

DESCRIPTION
       man  is the system's manual pager.  Each page argument given
       to man is normally the name of a program, utility  or  func‐
       tion.   The  manual page associated with each of these argu‐
       ments is then found and displayed.  A section, if  provided,
       will  direct man to look only in that section of the manual.
       The default action is to search in all of the available sec‐
       tions  following  a pre-defined order (see DEFAULTS), and to
       show only the first page found, even if page exists in  sev‐
       eral sections.

       The table below shows the section numbers of the manual fol‐
       lowed by the types of pages they contain.

       1   Executable programs or shell commands
       2   System calls (functions provided by the kernel)
       3   Library calls (functions within program libraries)
       4   Special files (usually found in /dev)
       5   File formats and conventions, e.g. /etc/passwd
       6   Games
       7   Miscellaneous  (including  macro  packages  and  conven‐
           tions), e.g. man(7), groff(7)
       8   System administration commands (usually only for root)
       9   Kernel routines [Non standard]

       A manual page consists of several sections.

       Conventional  section names include NAME, SYNOPSIS, CONFIGU‐
       RATION, DESCRIPTION, OPTIONS, EXIT STATUS, RETURN VALUE, ER‐
       RORS,  ENVIRONMENT,  FILES,  VERSIONS, CONFORMING TO, NOTES,
       BUGS, EXAMPLE, AUTHORS, and SEE ALSO.

       The following conventions apply to the SYNOPSIS section  and
       can be used as a guide in other sections.

       bold text          type exactly as shown.
       italic text        replace with appropriate argument.
       [-abc]             any  or  all arguments within [ ] are op‐
                          tional.
       -a|-b              options delimited by | cannot be used to‐
                          gether.
       argument ...       argument is repeatable.
       [expression] ...   entire  expression within  [ ] is repeat‐
                          able.

       Exact rendering may vary depending  on  the  output  device.
       For instance, man will usually not be able to render italics
       when running in a terminal, and will  typically  use  under‐
       lined or coloured text instead.

       The  command  or  function  illustration  is  a pattern that
       should match all possible invocations.  In some cases it  is
       advisable  to illustrate several exclusive invocations as is
       shown in the SYNOPSIS section of this manual page.

EXAMPLES
       man ls
           Display the manual page for the item (program) ls.

       man man.7
           Display the manual page for macro package man from  sec‐
           tion  7.   (This  is  an  alternative spelling of "man 7
           man".)

       man 'man(7)'
           Display the manual page for macro package man from  sec‐
           tion 7.  (This is another alternative spelling of "man 7
           man".  It may be more convenient when copying and  past‐
           ing  cross-references  to  manual  pages.  Note that the
           parentheses must normally be quoted to protect them from
           the shell.)

       man -a intro
           Display,  in succession, all of the available intro man‐
           ual pages contained within the manual.  It  is  possible
           to quit between successive displays or skip any of them.

       man -t bash | lpr -Pps
           Format  the  manual page for bash into the default troff
           or groff format and pipe it to  the  printer  named  ps.
           The default output for groff is usually PostScript.  man
           --help should advise as to which processor is  bound  to
           the -t option.

       man -l -Tdvi ./foo.1x.gz > ./foo.1x.dvi
           This command will decompress and format the nroff source
           manual page ./foo.1x.gz into a device independent  (dvi)
           file.   The  redirection  is  necessary  as  the -T flag
           causes output to be directed to stdout  with  no  pager.
           The  output  could be viewed with a program such as xdvi
           or further processed into  PostScript  using  a  program
           such as dvips.

       man -k printf
           Search  the short descriptions and manual page names for
           the keyword printf as regular expression.  Print out any
           matches.  Equivalent to apropos printf.

       man -f smail
           Lookup  the  manual  pages referenced by smail and print
           out the short descriptions of any found.  Equivalent  to
           whatis smail.

OVERVIEW
       Many  options  are available to man in order to give as much
       flexibility as possible to the user.  Changes can be made to
       the  search path, section order, output processor, and other
       behaviours and operations detailed below.

       If set, various environment variables  are  interrogated  to
       determine  the  operation of man.  It is possible to set the
       "catch-all" variable $MANOPT to any string in  command  line
       format,  with  the exception that any spaces used as part of
       an option's argument must be escaped (preceded  by  a  back‐
       slash).   man  will  parse  $MANOPT prior to parsing its own
       command line.  Those options requiring an argument  will  be
       overridden  by  the  same options found on the command line.
       To reset all of the options set in $MANOPT, -D can be speci‐
       fied  as  the  initial command line option.  This will allow
       man to "forget" about the options specified in $MANOPT,  al‐
       though they must still have been valid.

       Manual  pages are normally stored in nroff(1) format under a
       directory such as /usr/share/man.   In  some  installations,
       there  may also be preformatted cat pages to improve perfor‐
       mance.  See manpath(5) for details of where these files  are
       stored.

       This  package  supports  manual pages in multiple languages,
       controlled by your locale.  If your system did not set  this
       up  for you automatically, then you may need to set $LC_MES‐
       SAGES, $LANG, or another system-dependent environment  vari‐
       able to indicate your preferred locale, usually specified in
       the POSIX format:

       <language>[_<territory>[.<character-set>[,<version>]]]

       If the desired page is available in your locale, it will  be
       displayed in lieu of the standard (usually American English)
       page.

       If you find that the translations supplied with this package
       are not available in your native language and you would like
       to supply them, please contact the maintainer  who  will  be
       coordinating such activity.

       Individual  manual pages are normally written and maintained
       by the maintainers of the program, function, or other  topic
       that  they document, and are not included with this package.
hacker@man~searching-for-manuals:~$ man -k flag
bwviykhkny (1)       - print the flag!
dpkg-buildflags (1)  - returns build flags to use during package b...
Dpkg::BuildFlags (3perl) - query build flags
fegetexceptflag (3)  - floating-point rounding and exception handling
fesetexceptflag (3)  - floating-point rounding and exception handling
i386 (8)             - change reported architecture in new program...
ioctl_iflags (2)     - ioctl() operations for inode flags
linux32 (1)          - change reported architecture in new program...
linux64 (1)          - change reported architecture in new program...
pcap-config (1)      - write libpcap compiler and linker flags to ...
security_compute_av_flags (3) - query the SELinux policy database ...
security_compute_av_flags_raw (3) - query the SELinux policy datab...
set_matchpathcon_flags (3) - set flags controlling the operation o...
set_matchpathcon_invalidcon (3) - set flags controlling the operat...
set_matchpathcon_printf (3) - set flags controlling the operation ...
setarch (1)          - change reported architecture in new program...
setarch (8)          - change reported architecture in new program...
x86_64 (8)           - change reported architecture in new program...
hacker@man~searching-for-manuals:~$ bwviykhkny (1)
ssh-entrypoint: syntax error near unexpected token `1'
hacker@man~searching-for-manuals:~$ bwviykhkny 1
ssh-entrypoint: bwviykhkny: command not found
hacker@man~searching-for-manuals:~$ man bwviykhkny

CHALLENGE(1)             Challenge Commands            CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit
/flag
...skipping
              print the flag if NUM is 466

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The  repository  for  this dojo: <https://github.com/pwncol‐
       lege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                   May 2024                 CHALLENGE(1)
hacker@man~searching-for-manuals:~$ man bwviykhkny

CHALLENGE(1)             Challenge Commands            CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --bwviyk NUM
              print the flag if NUM is 466

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The  repository  for  this dojo: <https://github.com/pwncol‐
       lege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                   May 2024                 CHALLENGE(1)
hacker@man~searching-for-manuals:~$
hacker@man~searching-for-manuals:~$
hacker@man~searching-for-manuals:~$
hacker@man~searching-for-manuals:~$
hacker@man~searching-for-manuals:~$
hacker@man~searching-for-manuals:~$
hacker@man~searching-for-manuals:~$ /challenge/challenge --bwviyk 466
Correct usage! Your flag: pwn.college{4W6SbDwVN6Dviykh8kTGnQ7y0Nh.dZTM4QDLzQjN1czW}
hacker@man~searching-for-manuals:~$
```
I found in the man manual that we can use the `-k` argument to man to find the right manual for `challenge` command so:

I used the command `man -k flag` to search for flag key word in the different manuals headings and description and found `bwviykhkny` and then opened this manual using `man bwviykhkny` and found the `--bwviyk NUM` argument which will give me the flag if NUM=466

So finally I used the command `/challenge/challenge --bwviyk 466` to find the flag
