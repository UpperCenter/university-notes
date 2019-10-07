# PS4 System Information Report

- [PS4 System Information Report](#ps4-system-information-report)
  - [Storage Options](#storage-options)
  - [Hard Drive Information](#hard-drive-information)
  - [Types of Data Stored](#types-of-data-stored)
    - [File Structure](#file-structure)
    - [Partition Format](#partition-format)
  - [RAM Configuration](#ram-configuration)
  - [Blu-Ray Drive](#blu-ray-drive)
    - [File Structure:](#file-structure)
  - [External Storage](#external-storage)
    - [External File Structure](#external-file-structure)
  - [Citations](#citations)

## Storage Options

* HDD (Standard)
* SSD (Not Officially Supported)
* External storage is also available

## Hard Drive Information

* The standard PS4 has a 500GB, 5400 RPM, SATA II HDD (Default)
* The PS4 Pro has a 1TB version (Default)

## Types of Data Stored

* Games
* Applications
* Video
* Images

### File Structure

* Partition Format: UFS
* Capacity 500GB -12TB
* File Systems Supported: FAT32, exFAT

Firmware information:
- Name: ORBIS OS
- Based on: FreeBSD 9.0
- Platform: 64 bits (x86_64)


### Partition Format

| No | Device File | Z5K500 size | ST500LM012 size   | in bytes        | type                                   |
|:---|:-----------:|------------:|------------------:|----------------:|----------------------------------------|
| 1  | /dev/sdc17  | 1 GiB       | 1 GiB             | 1,073,741,824   | `80dd49e3-a985-4887-81de-1daca47aed90` |
| 2  | /dev/sdc31  | 16 GiB      | 16 GiB            | 17,179,869,184  | `3ef7290a-de81-4887-a11f-46fba765c71c` |
| 3  | /dev/sdc27  | 420.12 GiB  | 420.120117188 GiB | 451,100,540,928 | `c638477a-e002-4b57-a454-a27fb63a33a8` |
| 4  | /dev/sdc13  | 8 GiB       | 8 GiB             | 8,589,934,592   | `76a9a5b4-44b0-472a-bde3-3107472adee2` |
| 5  | /dev/sdc9   | 1 GiB       | 1 GiB             | 1,073,741,824   | `757a614b-6179-5361-6b61-6b6968617261` |
| 6  | /dev/sdc10  | 1 GiB       | 1 GiB             | 1,073,741,824   | `757a614b-6179-5361-6b61-6b6968617261` |
| 7  | /dev/sdc11  | 1 GiB       | 1 GiB             | 1,073,741,824   | `dc85025f-a694-4109-be44-fa0c063e8b81` |
| 8  | /dev/sdc12  | 1 GiB       | 1 GiB             | 1,073,741,824   | `dc85025f-a694-4109-be44-fa0c063e8b81` |
| 9  | /dev/sdc19  | 8 GiB       | 8 GiB             | 8,589,924,592   | `a71ff62d-1421-4dd9-935d-25dabd81bec5` |
| A  | /dev/sdc1   | 512 MiB     | 512 MiB           | 536,780,912     | `17800f17-b9e1-425d-b937-0119a0813172` |
| B  | /dev/sdc3   | 1 GiB       | 1 GiB             | 1,073,741,824   | `ccb52e94-ebef-48c4-a195-9e2da5b0292c` |
| C  | /dev/sdc5   | 16 MiB      | 16 MiB            | 16,777,216      | `145268bf-63ad-47c1-9378-9aacd9beed7c` |
| D  | /dev/sdc7   | 128 MiB     | 128 MiB           | 134,217,728     | `6e0c5310-8445-4066-b571-9b65fdb75935` |
| E  | /dev/sdc29  | 1 GiB       | 1 GiB             | 1,073,741,824   | `21e4dfb4-0040-4934-a037-ea9dc058eea6` |
| F  | /dev/sdc25  | 6 GiB       | 6 GiB             | 6,442,450,944   | `fdb5ede1-73c3-4c43-8c5b-2d3dcfcddff8` |


## RAM Configuration

|                                                                   | Value         |
|:------------------------------------------------------------------|---------------|
| Total Size:                                                       | 8GB           |
| Addressability:                                                   | unified       |
| Configuration / Bus-width:                                        | ?x?=256bit    |
| Channels:                                                         | 8x32bit       |
| Module Type:                                                      | GDDR5         |
| Speed (effective):                                                | 5500          |
| Cache:                                                            | N/A           |
| Bandwidth (Gbit/s):                                               | 176           |
| System Reserved / Application+Game Free (GB) / Flexible Memory:   | 2.5 / 4.5 / 1 |

## Blu-Ray Drive

### File Structure:

```
├─ PS4 
│   └─ UPDATE
│       └─ PS4UPDATE.PUP
│          
├─ app 
│   └─ Productcode
│           └─ app.pkg 
│          
├─ bd 
│   └─ param.sfo 
│       
└─ license 
    └─ rif
```

## External Storage

### External File Structure

```
├───*:\Root On Mass Storage
├───PS4
│    ├───SAVEDATA                 (Save Games)
│    │      └───0000000000000000  (default folder)
│    │               └───CUSA00001  (Save Game Folder)
│    │	                    └───savedata
│    │	                    └───savedata.bin
│    └───UPDATE  (PS4UPDATE.PUP System Firmware file)
│    │	                  
│    └───EXPORT
│             └───BACKUP 
│                   └───201504261757_00    (The folder with the backup chunks of the HDD, contains the date, the time and the backup number)
│                                ├───archive.dat  (4,194,240 KB)
│                                ├───archive0001.dat (4,194,240 KB)
│                                ├───archive0002.dat (4,194,240 KB)
│                                ├───archive0003.dat (4,194,240 KB)
│                                ├───archive0004.dat (4,194,240 KB)
│                                └───archive0005.dat (4,194,240 KB)
├───SHARE (Share recorded Exports)
│    ├───Screenshots
│    │     └───(Name Of Game)
│    │	          └───nameofgame.jpg
│    │	    └───Other
│    └────Video Clips
│         └───(Name Of Game)
│    	         └───nameofgame.mp4  
├───SHAREFACTORY                    (PS4 Movie Making Application)
│         └───MUSIC
├───(NAMEOFGAME)                  (Similar to SHAREFACTORY's folder)        
│         ├───image.png
│         ├───image.jpg
│         └───music.mp3 *?
├───Music
│         ├───music.mp3           ( Audio media can be played from a USB stick device, if these files are placed into a folder called "music"
│         ├───music.mp4             - Supported codec : AAC (2channel) and MP3 (2 channel)
│         ├───music.m4a             - Sampling Frequency: 22.05kHz、24kHz; 32kHz、44.1kHz、48kHz; 96kHz
│         └───music.3gp             - Playlist: .m3u, m3u8                                                                                     )
└───[MUSIC/PICTURE/VIDEO] *?
```

## Citations

+ [PS4 Dev Wiki](https://www.psdevwiki.com/ps4/Main_Page)

