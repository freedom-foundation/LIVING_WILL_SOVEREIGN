### DEFINITIONS
mandate - the manualy entered date of creation or release.
 fuzzydate - mandates may be fuzzy dates like so 20170000 these should be certain to the resolution and do not discredit the date yet may be used to deduce a sequence of events, chronology. 
mantitle - the title the author applies.
mansize - the veritas file size as it is in bits or greater.
wordcount - the count of pages, lines, words, characters of a document.
encoding - means the way the machine stores the data of a document
checksum - means a mathematical operation either by hand or usually machine used to check the integrity of a file.
type - means a machine specification for how to handle the data of a document


The development points of My development cycle are in ALL_CAPS.
ALPHA - means created yet in the process of adding and editing.
BETA - means it has been finished but needa to be proofread peer reviewed or checked for bugs. Ready to be tested.
RELEASE - means finished having been tested for Quality and Assurance, and ready to print, send, or use.
RELEASE PRINT - means a finished document ready to print for a hardcopy, publishing, or signature. 
RELEASE ARCHIVE - means a finished document having been checked over after at least one release print cycle. Maybe having been reproduced from a print release. Must be sourced from a release print meaning it is the same as a physical hardcopy. A release archive is then a veritas libre-sourcecode having a detachable FIC file for Peeranoia. 
FIC - means File Integrity Check(ing) and is used as the accompanying file of a release archive for PEERANOIA having the filename extension .FIC

The files should be saved thrice yet four and five times with differing names according to sort orders name and date. When sorted by filename having the information of other sort targets in the filename already accomplishes the sorting while providing the benefits of redundancy. This filename conventions specifies how I name files. This is a late ALPHA version meaning it explains what I have already been doing. The sort options are name, size, date, type.  In My DEVELOPER mode size is excluded because when sorting by size it is usually having to do with disk space limitations and another redundant copy to sort by size is counter intuitive. Type is excluded[1] from the three filenames because it is the same as the extension for each redundant file and shows at the end of the filename such as ".txt". Type can be done at an archive RELEASE stage: My RELEASE mode . Each section of information is to be separated by a period ".". Beginningbwith targets date and name for my developer mode in the ALPHA stage of my development cycle.  The name is the title of the document. Any whitespaces in the title are converted to underscores for the title in the filename. Such as "LIVING_WILL_SOVEREIGN". Some punctuation may be omited for the title only as it appears in the filename having converted whitespaces to underscores. As a general rule of omiting punctuation it standardizes the rule of excluding period which can be punctuation. Special characters within the title should be avoided because they can cause data loss when filesystems do not handle these. Specificly colon is allowed on EXT while not FAT and a copy operation may skip filenames having a colon. To avoid these they may be omitted or spelled. Such as "ampersand" as in "Politicks_ampersand_War" for "Politicks & War". Title shall be the same as the title which is self referenced within the document. The title shall be underlined in the document header. If there is no title then part of the first line shall be used as a title and optionally part of the last line after it. Such were "HAVING_SOUND_MIND-FAITHFULLY_CARRIED_OUT". Here the document begins with identity of the author so that part was skipped, using an intelligent heuristic, to focus on the document content as title and not the author. The author should be a separate section of information in directories containing files having multiple authors, as such the author's identity should not be used as a title. Using an intelligent heuristic about three words may be selected to use for a title in the filename. Using about three words from the first and last lines can logicly chain link multipage documents when the pages are separate files. Chain-link means the last part of the preceeding page is the beginning of the next page. This works well when editing OCR generated files from photos. Continuing on with the second sort target date. 
### mandates
Sort by date - For development mode the sort target to focus on is date. The date shall be in ISO-8601 as such 20241210. In the development process the two filename sort targets to be saved are title and date. Filename by date works well for versioning files during the process of creation and editing. When the date is entered manualy it can be called a mandate in the filename in contrast to the machine tagged timestamps of the file info. Mandate because it is manualy entered or entered by the man. The date shall be included in the header/footer in the document. The targetted requirement is at least the year. Such as "2017". The mandate should correspond to the creation or release date and when the creation date is not exactly known zeros may be used to fill in the unknown sections thus forming a fuzzy-date. Such as 
```
20170000.SOVEREIGN.txt
```
Time is optional. Time shall be in 24 hour format with the timezone at the end such as CST. The order is YYYYMMDDHHMMSSUTC. After development mode is release mode. 
### My RELEASE mode
Release mode means the document is finished and ready to send. As with a letter which is ready to be delivered. The sort target size may be applied in the filename at this point and also the sort target type in reverse order.
 The sort target size may be applied in the filename at the point of BETA when undergoing testing I would test from the 2443B.20170000.LIVING_WILL_SOVEREIGN file.
#### mansize
Size has to do with the time it takes to transmit or the limitations of the receiver. Size shall be in bytes with a capital B. Such as 2334B. When no alphabetic character is used this should indicate the filesize is specified in bits and not bytes however most filesystems store only in Byte-sized blocks therefor bits generally become inaccurate for this entering the size in bits is generally not used but only in uncommon usage. The size entered may be called the man-size in contrast with the machine which pads the data to fit Byte-size filesystem blocks. When using Bytes the mansize and machine tagged size coencide. Only when the manssize is specified in bits can the filename show the machine has altered the filesize. Optionally M or G may be used for megabytes and gigabytes but generally avoided because M often uses a decimal point which may be confused as a separator in the filename. Since size is machine calculated it shall be referenced just before the checksum but after the wordcount. After the combinations of sort order: date.title.wordcount.size.checksum, title.date.wordcount.size.checksum, size.checksum.title.date.wordcount, in this order where size is the last combination then the wordcount shall be in the filename.
#### wordcount
Wordcount shall use the order from nano (pages-)lines-words(-charsnowhitesspace)-characters. Pages is optional so is charsnowhitespace. The title shall be the same as the title which is self referenced within the doc. The mantitle shall be taken from the self-reference in the text, the title underlined in the document header, or select about three words from the first line and last line for chanlinking files as pages. The date shall be in ISO-8601. Such as 20241210.

```2017.LIVING_WILL_SOVEREIGN.2334B.a4c69ded1afb670560b39cd48937d4c2.txt```

```LIVING_WILL_SOVEREIGN.2017.2334B.a4c69ded1afb670560b39cd48937d4c2.txt```
#### checksum
Checksums should be in lowercase, or the preferred case of insensitivity. Lowercase is preferred when not using DOS compat. Checksums come just before the extension by order of depth and always begin with an md5sum further depth of checksums are optional. The order of checksums by depth from left to right is: md5sum, sha1sum, sha224sum, sha256sum, sha512sum. Such as md5sum(.sha224sum).txt where the parenthesis are optionly omited.```SOVEREIGN.A4C69DED1AFB670560B39CD48937D4C2.TXT```

#### encoding
As for encoding such as ASCII, ISO-8859-1, and UTF-8 this is specified as a section appended after wordcount or prepended before type. ```My_file.ASCII.txt``` or ```My_file.5.500.5000.ASCII.checksum.txt```

### RELEASE ARCHIVE
Release files may be converted to DOS compatible filenames for maximum compatibility. For DOS compatibility filenames shall be eight alphanumeric characters and may include underscore followed by a period and three alphanumeric character extension describing the filetype. When the filesystem is case insensitive ALL_CAPS should be preferred Such as ALL_CAPS.TXT

Release files may be copied from the type sort target with the order reversed so the last section becomes the eight alphanumeric character filename as so
```txt.ASCII.2334B.a4c69ded1afb670560b39cd48937d4c2.20170000000000UTC.LIVING_WILL_SOVEREIGN``` becomes ```SOVEREIG.TXT```

Note: When I shall select a title bear in mind the final word shall be parsed by a script to become the DOS compat. filename. 

All of the file information can then be exported into a second info file such as SOVEREIG.FIC the RELEASE ARCHIVE .FIC file would be the information file stored on Peeranoia_framework storage network it would be a PEERANOIA FIC file.
Note: By the time of an RELEASE ARCHIVE the wordcount shall have been checked manuly and counted by hand from the RELEASE PRINT.
### benefits
Redundant copies of files by using my naming conventions of multiple sort orders have benifits. The benifits of redundant copies of files are as follows. First it may avoid corruption. The efficacy of the benifits varies according to the physical medium used for storage. Magnetic disk platters and solid state storage differ. However, when using redundant copies, the physical location of the data stored on disk for each filename has different locations . If a sector goes bad at a location the document is stored it could not corrupt another having a different filename because another filename is data at a different location on disk. When a script is used to name files if the physical storage medium uses sequential writing it is recommended to write a hugefile in order to cause the locations of the data on disk to separate. After the files are written the hugefile may be deleted.

[1]: There may be benifits to writing a file by type first because automatic indexing would not register the filetype. When the type is written the order of sections of information should be reversed type.checksum.size.date.title or checksum.size.date.title.
 Another way to avoid automatic indexing is to use checksum section only for filename.
