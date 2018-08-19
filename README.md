# MFC-CLI provides an external API for basic wallet functions

## Prerequisites

You will need Window or Linux. Use a virtual machine if you have a Mac. Ubuntu 14 and 16 are supported. Ubuntu 17 is not supported.

Install [.NET Core](https://www.microsoft.com/net/download/core).

On Linux, install the LevelDB and SQLite3 dev packages. E.g. on Ubuntu:

```sh
sudo apt-get install libleveldb-dev sqlite3 libsqlite3-dev libunwind8-dev

```

On Windows, use the [Neo version of LevelDB](https://github.com/neo-project/leveldb).

## Download pre-compiled binaries

See also [official docs](https://mfchain.com). Download and unzip [latest release](https://github.com/MFChain/mfc-cli/releases).

```sh
dotnet mfc-cli.dll
```

## Compile from source

Clone the mfc-cli repository.

```sh
cd mfc-cli
dotnet restore
dotnet publish -c Release
```
In order to run, you need version 1.1.2 of .Net Core. Download the SDK [binary](https://www.microsoft.com/net/download/linux).

Assuming you extracted .Net in the parent folder:

```sh
../dotnet bin/Release/netcoreapp1.0/mfc-cli.dll .
```

## Usage

See [documentation](https://mfchain.com). E.g. try `show state` or `create wallet wallet.db3`.
