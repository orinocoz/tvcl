# tvcl
Command line interface for TV Shows Tracking
![](https://dl.dropboxusercontent.com/u/1995551/misc/tvcl.png)

# Intro
This small tool is a CLI for [http://thetvdb.com/](http://thetvdb.com/) API. It allows to track tv shows you follow and the episodes you didn't watch yet.

# Features
- Lookup for shows
- Viewing episodes titles, air dates, overview, and more
- Marking episodes as wacthed
- Showing episodes you didn't watch yet

# Install

```bash
$ npm install tvcl -g
```

`tvcl` uses the [http://thetvdb.com/](http://thetvdb.com/) API. In order to use it you should [get an API key](http://thetvdb.com/?tab=apiregister) and put it into `THETVDB_API_KEY` environment variable.

# Usage

Lookup the series title:
```bash
$ tvcl lookup the simpsons
```
(you can use `search` alias)

Add the series to local database by id:
```bash 
$ tvcl add {id}
```

List added series:
```bash
$ tvcl list
```

View episodes (--wo stands for "with overview"):
```bash
$ tvcl view {id} --wo
```
(you can use `show` alias)

Mark episode as watched:
```
$ tvcl watch {epid}
```

Mark all episodes till the specified as watched:
```bash
$ tvcl watch-till {epid}
```
(you can use `wt` alias)

Show the not-watched-yet episoded:
```
$ tvcl remained 
```
or just
```
$ tvcl
```
