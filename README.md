# Useful commands
Useful commands with Linux and Windows

## Table of contents

* [1. Unzip .zip file in Linux](#unzip-zip-file-in-linux)
* [2. Unzip .zip file in Linux](#unzip-zip-file-in-linux)
* 
## 🔻Unzip .zip file in Linux

#### ➤ Unzip normal file
```
kiosec@cyberlab:~#7z x test.zip

7-Zip [64] 16.02 : Copyright (c) 1999-2016 Igor Pavlov : 2016-05-21
p7zip Version 16.02 (locale=en_US.UTF-8,Utf16=on,HugeFiles=on,64 bits,128 CPUs AMD EPYC 7543 32-Core Processor                 (A00F11),ASM,AES-NI)

Scanning the drive for archives:
1 file, 10870 bytes (11 KiB)

Extracting archive: test.zip
--
Path = test.zip
Type = zip
Physical Size = 10870

    
Enter password (will not be echoed):
Everything is Ok         

Size:       271360
Compressed: 10870
```

#### ➤ Unzip .zip file with space (Access control.zip)

```
kiosec@cyberlab:~#7z x Access\ Control.zip

7-Zip [64] 16.02 : Copyright (c) 1999-2016 Igor Pavlov : 2016-05-21
p7zip Version 16.02 (locale=en_US.UTF-8,Utf16=on,HugeFiles=on,64 bits,128 CPUs AMD EPYC 7543 32-Core Processor                 (A00F11),ASM,AES-NI)

Scanning the drive for archives:
1 file, 10870 bytes (11 KiB)

Extracting archive: Access Control.zip
--
Path = Access Control.zip
Type = zip
Physical Size = 10870

    
Enter password (will not be echoed):
Everything is Ok         

Size:       271360
Compressed: 10870
```

## 🔻Read .pst file using Linux (ex: Access Control.pst file)

#### ➤ Install readpst
```
kiosec@cyberlab:~#sudo apt-get install readpst
kiosec@cyberlab:~#sudo apt-get install pst-utils
```

#### ➤ Open .pst file
```
kiosec@cyberlab:~#readpst -tea -m Access\ Control.pst
Opening PST file and indexes...
Processing Folder "Deleted Items"
	"Access Control" - 2 items done, 0 items skipped.
```

#### ➤ Move to new directory created
```
kiosec@cyberlab:~#cd 'Access control'
```

#### ➤ Read message
```
kiosec@cyberlab:~#dir
2.eml  2.msg

kiosec@cyberlab:~#cat 2.eml
<...>
```

