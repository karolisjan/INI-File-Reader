# INI File Reader

A simple parser of .INI files.

## Usage

#### Example .INI file

```
[Options]
iVar = 1234
sVar = some_text
fVar = 1.234
bVar = false
```

#### Reading .INI file in C++

```
#include "ini_reader.hpp"

...

IniFile ini_file("location\of\file.ini");

int iVar = ini_file.Read<int>("Options", "iVar");
std::string = ini_file.Read<std::string>("Options", "sVar");
float fVar = ini_file.Read<float>("Options", "fVar");
bool bVar = ini_file.Read<bool>("Options", "bVar");

ini_file.Close();
```
