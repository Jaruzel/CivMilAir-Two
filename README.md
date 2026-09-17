# TL;DR

A large set of files saved and converted from 100 floppy disks that were created on a Canon StarWriter in the late 1990s, obtained by me from eBay. The files are the work of someone who (probably) died without seeing the 25 years of his work fully published. The files are lists of aircraft that started off with Military designations but later got re-designated with Civilian numbers. There are about 500,000 craft listed.

Read [the original authors introduction](CivIntro.md) for more information.

# Background

At some point in early 2025 I won an eBay auction for a set of used floppy disks. As a retro computing enthusiast, I am always on the lookout for good quality used floppy disks. 

The disks I won had not been wiped, and contained dos-like files. Each disk had a carefully written label saying 'CivMilAir' follow by a range of numbers.

At this point, I had two choices, wipe the disks and just use them, or try to extract the information and see what this 'CivMilAir' stuff is. I of course chose the latter. Everyone loves a silly project right?

Further investigation revealed that the disks were used on a Canon StarWriter Electric Word-processor. This machine read and wrote files onto standard DOS formatted 720k 3.5" floppies. 

However the file format (and filenames) were proprietary to the Canon. DOS could not see all of the files, and the contents of the files it could see were not plain text.

After a bit of Googling, I found a couple of Canon file convertors. Unfortunately neither were suitable for my purpose, nor did they do batch conversion. I had 100 disks with many files on them. No way I wanted to do that manually. Nor did it solve the missing (invisible to DOS) files.

So, I wrote a custom disk imager to rip the disks to standard .IMA files. This involved learning WAY more about the FAT disk format than I ever needed to know.

After that, I wrote a file extractor. This took each IMA file and extracted all the files, renaming any that had invalid DOS file names.

From those 100 disks, I ended up with over 2,500 files.

Next step was to write a basic Canon StarWriter file format converter. I didn't go all on this, just enough to be able to read the content of the files in a text editor. 

# The Original Author

Most of the files were lists of Aircraft information, but some were personal letters to other people, written by the owner of these disks. I have of course NOT uploaded any of those to this collection (and I have since deleted all of them). However from reading the letters I gleaned the following information about this collection:

- The Author was John R Ryder (I'm including his name, as this is HIS collection)
- He spent 25 years building these lists.
- He previous published a book called 'Civmilair – British Civil Registration/Military Serial Cross Reference (from 1919)' in 1984
- This collection of lists is an updated version of that book
- He hoped to get it all published again, but couldn't get interest (The internet had basically killed any interest in hard-copy books like this)
- He hadn't realised that the Canon was proprietary, and that the files it created couldn't easily be shared.
- Based on the personal information I read, and that the disks were being sold by a house clearance company, I can only assume he died (old age), without these new lists ever seeing the light of day.

Personally, I feel sad that all his efforts went unseen. This was what drove me to convert everything and upload it all here. Even if no-one ever sees them, at least they are now available should they contain information not recorded elsewhere (The author was clear in some of his letters that he never wanted any money from his efforts). I am not an aviation enthusiast, so I do not know how useful any of this is, to be honest.

# The Collection

All the text files are converted directly from the extracted Canon disks. As mentioned, they are only partially converted - enough to be read or parsed further.

- [US.ZIP](US.ZIP) : 2,213 Files
- [CIV.ZIP](CIV.ZIP) : 111 files
- [DH.ZIP](DH.ZIP) : 23 files
- [MISC.ZIP](MISC.ZIP) : 23 files

I did write a tool to merge all the *US___.TXT* files into a single CSV of data, but the time involved and the many, many, formatting edge cases made it unpractical for me continue converting the *CIV___.TXT*, *AU___.TXT*, and *DH___.TXT* files, etc.  That said, the US set is over 80% of the data (347,000 entries).

The US merged list is [US-FULL.CSV](US-FULL.CSV).

# Finally

To reiterate, the contents of these files are NOT MY WORK. I only extracted, converted and merged them. 

If anyone has any issue with these lists being published online, please contact me, and I will consider taking the collection down.




