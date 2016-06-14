# fs1nspector
File system visualisation. 

List file system content, starting from a given path.

Collects informations about files.

Creates image presenting files based on given critera. 

This should ideally help in forensic work to have an idea what type of data file system contains at first glance.

### Example
Random color for each file extension. 

Gray ==> extension unknown or missing.

![image](https://raw.githubusercontent.com/chaoos-theory/fs1nspector/master/test.jpg)


#### TODO
Include criteria specification that will allow to highlight specific files based on:
- file type
- given file type category (as in image, media, documents, iso, etc)
- size limit over or under
- modification in last x days, week, month, year
- owned by specific user
- hidden directly ( preciding . in filename) or indirectly (parent folder hidden)
- is executable (not sure if possible to differentiate other than by reading attributes in which case exe/msi will be ommieted on linux)
- 0 size
- pattern in name
- pattern in full path (including name)

Allow file type coloring based on config file read at startup. 
