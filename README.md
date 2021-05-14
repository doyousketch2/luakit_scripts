# luakit_scripts
lua &amp; css config for luakit browser

---

most of the .css removes headers & footers, stuff like that

luakit runs faster if you clear unused cache that's just been sitting there for 2 weeks

add to your  `~/.bash_aliases`  then use **lk** to auto clear cache && call luakit

    function lk() {  ##  tidy cache, then run luakit
      clear              ##  mtime = days since modified
      find ~/.cache/luakit/ -mtime +14 -exec rm {} \; 2>/dev/null
      luakit  ##  don't fill commandline w/ errors about dirs  ^^
    }

---
don't think I've ever used "autoscroll" but it looked neat, so it's in my .config dir
