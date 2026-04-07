# Installing-Mongo-DB-in-Mac

Last login: Tue Apr  7 08:41:14 on ttys000
viveksparmar@Viveks-MacBook-Air ~ % /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
==> Checking for `sudo` access (which may request your password)...
Password:
==> This script will install:
/opt/homebrew/bin/brew
/opt/homebrew/share/doc/homebrew
/opt/homebrew/share/man/man1/brew.1
/opt/homebrew/share/zsh/site-functions/_brew
/opt/homebrew/etc/bash_completion.d/brew
/opt/homebrew
/etc/paths.d/homebrew

Press RETURN/ENTER to continue or any other key to abort:
==> /usr/bin/sudo /usr/sbin/chown -R viveksparmar:admin /opt/homebrew
==> Downloading and installing Homebrew...
remote: Enumerating objects: 151, done.
remote: Counting objects: 100% (83/83), done.
remote: Compressing objects: 100% (21/21), done.
remote: Total 151 (delta 64), reused 72 (delta 62), pack-reused 68 (from 3)
==> /usr/bin/sudo /bin/mkdir -p /etc/paths.d
==> /usr/bin/sudo tee /etc/paths.d/homebrew
/opt/homebrew/bin
==> /usr/bin/sudo /usr/sbin/chown root:wheel /etc/paths.d/homebrew
==> /usr/bin/sudo /bin/chmod a+r /etc/paths.d/homebrew
==> Updating Homebrew...
Updated 1 tap (homebrew/core).
==> Installation successful!

==> Homebrew has enabled anonymous aggregate formulae and cask analytics.
Read the analytics documentation (and how to opt-out) here:
  https://docs.brew.sh/Analytics
No analytics data has been sent yet (nor will any be during this install run).

==> Homebrew is run entirely by unpaid volunteers. Please consider donating:
  https://github.com/Homebrew/brew#donations

==> Next steps:
- Run brew help to get started
- Further documentation:
    https://docs.brew.sh

viveksparmar@Viveks-MacBook-Air ~ % brew --version
Homebrew 5.1.4
viveksparmar@Viveks-MacBook-Air ~ % brew tap mongodb/brew
==> Tapping mongodb/brew
Cloning into '/opt/homebrew/Library/Taps/mongodb/homebrew-brew'...
remote: Enumerating objects: 1787, done.
remote: Counting objects: 100% (719/719), done.
remote: Compressing objects: 100% (307/307), done.
remote: Total 1787 (delta 614), reused 423 (delta 412), pack-reused 1068 (from 2)
Receiving objects: 100% (1787/1787), 399.09 KiB | 2.27 MiB/s, done.
Resolving deltas: 100% (1115/1115), done.
Tapped 13 formulae (32 files, 512.4KB).
viveksparmar@Viveks-MacBook-Air ~ % brew install mongodb-community
==> Fetching downloads for: mongodb-community
✔︎ Bottle Manifest fmt (12.1.0)                                                               Downloaded    7.3KB/  7.3KB
✔︎ Bottle fmt (12.1.0)                                                                        Downloaded  282.9KB/282.9KB
✔︎ Bottle Manifest ada-url (3.4.4)                                                            Downloaded    8.7KB/  8.7KB
✔︎ Bottle ada-url (3.4.4)                                                                     Downloaded  345.6KB/345.6KB
✔︎ Bottle Manifest brotli (1.2.0)                                                             Downloaded    8.0KB/  8.0KB
✔︎ Bottle Manifest c-ares (1.34.6)                                                            Downloaded    7.5KB/  7.5KB
✔︎ Bottle c-ares (1.34.6)                                                                     Downloaded  304.0KB/304.0KB
✔︎ Bottle Manifest hdrhistogram_c (0.11.9)                                                    Downloaded    7.8KB/  7.8KB
✔︎ Bottle hdrhistogram_c (0.11.9)                                                             Downloaded   43.6KB/ 43.6KB
✔︎ Bottle Manifest libnghttp2 (1.68.1)                                                        Downloaded    7.3KB/  7.3KB
✔︎ Bottle libnghttp2 (1.68.1)                                                                 Downloaded  214.4KB/214.4KB
✔︎ Bottle Manifest libnghttp3 (1.15.0)                                                        Downloaded    7.3KB/  7.3KB
✔︎ Bottle libnghttp3 (1.15.0)                                                                 Downloaded  188.8KB/188.8KB
✔︎ Bottle Manifest libngtcp2 (1.22.0)                                                         Downloaded    9.7KB/  9.7KB
✔︎ Bottle libngtcp2 (1.22.0)                                                                  Downloaded  407.3KB/407.3KB
✔︎ Bottle Manifest libuv (1.52.1)                                                             Downloaded    7.5KB/  7.5KB
✔︎ Bottle libuv (1.52.1)                                                                      Downloaded  375.7KB/375.7KB
✔︎ Bottle Manifest llhttp (9.3.1)                                                             Downloaded    7.2KB/  7.2KB
✔︎ Bottle llhttp (9.3.1)                                                                      Downloaded   36.7KB/ 36.7KB
✔︎ Bottle Manifest simdjson (4.6.1)                                                           Downloaded    7.4KB/  7.4KB
✔︎ Bottle Manifest readline (8.3.3)                                                           Downloaded   10.0KB/ 10.0KB
✔︎ Bottle Manifest sqlite (3.51.3)                                                            Downloaded   11.4KB/ 11.4KB
✔︎ Bottle Manifest uvwasi (0.0.23)                                                            Downloaded    8.3KB/  8.3KB
✔︎ Bottle brotli (1.2.0)                                                                      Downloaded  793.5KB/793.5KB
✔︎ Bottle simdjson (4.6.1)                                                                    Downloaded    1.4MB/  1.4MB
✔︎ Bottle Manifest node (25.9.0_1)                                                            Downloaded   31.1KB/ 31.1KB
✔︎ Bottle Manifest mongosh (2.8.2)                                                            Downloaded   66.1KB/ 66.1KB
✔︎ Bottle uvwasi (0.0.23)                                                                     Downloaded   70.0KB/ 70.0KB
✔︎ Bottle readline (8.3.3)                                                                    Downloaded  757.9KB/757.9KB
✔︎ Bottle sqlite (3.51.3)                                                                     Downloaded    2.4MB/  2.4MB
✔︎ Bottle node (25.9.0_1)                                                                     Downloaded   18.5MB/ 18.5MB
✔︎ Formula mongodb-database-tools (100.16.0)                                                  Verified     71.0MB/ 71.0MB
✔︎ Formula mongodb-community (8.2.7)                                                          Verified     80.3MB/ 80.3MB
✔︎ Bottle mongosh (2.8.2)                                                                     Downloaded   22.4MB/ 22.4MB
==> Installing mongodb-community from mongodb/brew
==> Installing dependencies for mongodb/brew/mongodb-community: mongodb/brew/mongodb-database-tools, fmt, ada-url, brotli, c-ares, hdrhistogram_c, libnghttp2, libnghttp3, libngtcp2, libuv, llhttp, simdjson, readline, sqlite, uvwasi, node and mongosh
==> Installing mongodb/brew/mongodb-community dependency: mongodb/brew/mongodb-database-tools
🍺  /opt/homebrew/Cellar/mongodb-database-tools/100.16.0: 16 files, 135.1MB, built in 3 seconds
==> Installing mongodb/brew/mongodb-community dependency: fmt
==> Pouring fmt--12.1.0.arm64_tahoe.bottle.tar.gz
🍺  /opt/homebrew/Cellar/fmt/12.1.0: 29 files, 1MB
==> Installing mongodb/brew/mongodb-community dependency: ada-url
==> Pouring ada-url--3.4.4.arm64_tahoe.bottle.tar.gz
🍺  /opt/homebrew/Cellar/ada-url/3.4.4: 55 files, 1.3MB
==> Installing mongodb/brew/mongodb-community dependency: brotli
==> Pouring brotli--1.2.0.arm64_tahoe.bottle.tar.gz
🍺  /opt/homebrew/Cellar/brotli/1.2.0: 33 files, 1.9MB
==> Installing mongodb/brew/mongodb-community dependency: c-ares
==> Pouring c-ares--1.34.6.arm64_tahoe.bottle.tar.gz
🍺  /opt/homebrew/Cellar/c-ares/1.34.6: 176 files, 1MB
==> Installing mongodb/brew/mongodb-community dependency: hdrhistogram_c
==> Pouring hdrhistogram_c--0.11.9.arm64_tahoe.bottle.1.tar.gz
🍺  /opt/homebrew/Cellar/hdrhistogram_c/0.11.9: 22 files, 172.8KB
==> Installing mongodb/brew/mongodb-community dependency: libnghttp2
==> Pouring libnghttp2--1.68.1.arm64_tahoe.bottle.tar.gz
🍺  /opt/homebrew/Cellar/libnghttp2/1.68.1: 14 files, 757KB
==> Installing mongodb/brew/mongodb-community dependency: libnghttp3
==> Pouring libnghttp3--1.15.0.arm64_tahoe.bottle.tar.gz
🍺  /opt/homebrew/Cellar/libnghttp3/1.15.0: 20 files, 603.6KB
==> Installing mongodb/brew/mongodb-community dependency: libngtcp2
==> Pouring libngtcp2--1.22.0.arm64_tahoe.bottle.tar.gz
🍺  /opt/homebrew/Cellar/libngtcp2/1.22.0: 21 files, 1.4MB
==> Installing mongodb/brew/mongodb-community dependency: libuv
==> Pouring libuv--1.52.1.arm64_tahoe.bottle.tar.gz
🍺  /opt/homebrew/Cellar/libuv/1.52.1: 35 files, 1.3MB
==> Installing mongodb/brew/mongodb-community dependency: llhttp
==> Pouring llhttp--9.3.1.arm64_tahoe.bottle.tar.gz
🍺  /opt/homebrew/Cellar/llhttp/9.3.1: 13 files, 160.2KB
==> Installing mongodb/brew/mongodb-community dependency: simdjson
==> Pouring simdjson--4.6.1.arm64_tahoe.bottle.tar.gz
🍺  /opt/homebrew/Cellar/simdjson/4.6.1: 19 files, 7.9MB
==> Installing mongodb/brew/mongodb-community dependency: readline
==> Pouring readline--8.3.3.arm64_tahoe.bottle.tar.gz
🍺  /opt/homebrew/Cellar/readline/8.3.3: 56 files, 2.7MB
==> Installing mongodb/brew/mongodb-community dependency: sqlite
==> Pouring sqlite--3.51.3.arm64_tahoe.bottle.tar.gz
🍺  /opt/homebrew/Cellar/sqlite/3.51.3: 13 files, 5.2MB
==> Installing mongodb/brew/mongodb-community dependency: uvwasi
==> Pouring uvwasi--0.0.23.arm64_tahoe.bottle.1.tar.gz
🍺  /opt/homebrew/Cellar/uvwasi/0.0.23: 15 files, 289KB
==> Installing mongodb/brew/mongodb-community dependency: node
==> Pouring node--25.9.0_1.arm64_tahoe.bottle.tar.gz
🍺  /opt/homebrew/Cellar/node/25.9.0_1: 1,889 files, 78MB
==> Installing mongodb/brew/mongodb-community dependency: mongosh
==> Pouring mongosh--2.8.2.arm64_tahoe.bottle.tar.gz
🍺  /opt/homebrew/Cellar/mongosh/2.8.2: 16,805 files, 107.8MB
==> Installing mongodb/brew/mongodb-community
==> Caveats
To start mongodb/brew/mongodb-community now and restart at login:
  brew services start mongodb/brew/mongodb-community
==> Summary
🍺  /opt/homebrew/Cellar/mongodb-community/8.2.7: 12 files, 256.6MB, built in 2 seconds
==> Running `brew cleanup mongodb-community`...
Disable this behaviour by setting `HOMEBREW_NO_INSTALL_CLEANUP=1`.
Hide these hints with `HOMEBREW_NO_ENV_HINTS=1` (see `man brew`).
==> Caveats
==> mongodb-community
To start mongodb/brew/mongodb-community now and restart at login:
  brew services start mongodb/brew/mongodb-community
viveksparmar@Viveks-MacBook-Air ~ % brew services start mongodb/brew/mongodb-community
==> Successfully started `mongodb-community` (label: homebrew.mxcl.mongodb-community)
viveksparmar@Viveks-MacBook-Air ~ % mongosh
Current Mongosh Log ID:	69d47717abba91fb1738bf98
Connecting to:		mongodb://127.0.0.1:27017/?directConnection=true&serverSelectionTimeoutMS=2000&appName=mongosh+2.8.2
Using MongoDB:		8.2.7
Using Mongosh:		2.8.2

For mongosh info see: https://www.mongodb.com/docs/mongodb-shell/


To help improve our products, anonymous usage data is collected and sent to MongoDB periodically (https://www.mongodb.com/legal/privacy-policy).
You can opt-out by running the disableTelemetry() command.

------
   The server generated these startup warnings when booting
   2026-04-07T08:46:29.463+05:30: Access control is not enabled for the database. Read and write access to data and configuration is unrestricted
------

test> use chitkara
switched to db chitkara
chitkara> db.createcollection("atn")
TypeError: db.createcollection is not a function
chitkara> db.createCollection("atn")
{ ok: 1 }
chitkara> db.atn.insertOne({
|   name: "Vivek",
|   email: "vivek@example.com",
|   mobile: "9876543210"
| })
{
  acknowledged: true,
  insertedId: ObjectId('69d47747abba91fb1738bf99')
}
chitkara> db.atn.find()
[
  {
    _id: ObjectId('69d47747abba91fb1738bf99'),
    name: 'Vivek',
    email: 'vivek@example.com',
    mobile: '9876543210'
  }
]
chitkara> show dbs
admin     40.00 KiB
chitkara  40.00 KiB
config    12.00 KiB
local     40.00 KiB
chitkara> show collections
atn
chitkara> 
