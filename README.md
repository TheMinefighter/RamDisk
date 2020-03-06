# RamDisk
**RamDisk** is a library for create virtual disk drive on system memory (using [ImDisk](http://www.ltr-data.se/opencode.html/#ImDisk)) which supports Windows NT/2000/XP/Vista/7/8/8.1/10 and Windows Server 2003/2003 R2/2008/2008 R2/2012/2012 R2, 32 and 64 bit editions.

## Get Started

### 1. Install Package

```
PM> Install-Package RamDisk
```

### 2. Use it

**Mount** a virtual disk drive for example size : 512MB and fileSystem : NTFS and name : 'Z' and label : "RamDisk".

```csharp
RamDisk.Mount(512, FileSystem.NTFS, 'Z', "RamDisk");
//or simpler (other parameters except size has default value)
RamDisk.Mount(512);
```

Then **Unmount** drive name : 'Z'

```csharp
RamDisk.Unmount('Z');
//or simpler (drive name has default value 'Z')
RamDisk.Unmount();
```

## License

RamDisk is Copyright © 2020 [Mohammd Javad Ebrahimi](https://github.com/mjebrahimi) under the MIT license.