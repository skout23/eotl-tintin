# eotl-tintin
some of my tintin related stuff... YMMV

## useful EoTL links
- http://www.eotl.org
- http://eotl.borkweb.com
- http://eotl.pbworks.com
- http://www.bogleg.com/eotl

## useful tintin++ links
- https://github.com/borkweb/tintin-eotl
- https://tintinplusplus-unoffical-documentation.readthedocs.io/en/latest/contents/features/mapper/01_getting-started.html
- https://tintin.sourceforge.io/manual/map.php
- https://tintin.sourceforge.io/forum/

## the tintin scripts
- more to come once I classify and cleanup.
```
tt++ setup.tin
```
## Startup will check for Guild and Spec 
- Wait a few seconds for your score to display
- Guild and Spec to be loaded after they are parsed (will take about 3 seconds after login/reconnect)
```
> 
After the Score... here we go
Checking Guild ...
Found: Fighter
Loading ./lib/guilds/Fighter.tin ....
Checking Spec ...
Found: Berserker
Loading ./lib/specs/Berserker.tin ....
```

## set your default target 
- default is `monster` if you want something else
```
tt human
tt dragon
etc etc
```

## private scripts
- put any scripts you want kept private in `lib/private/private.tin`
- or anywhere you like.

## the mapper
```
#help map
#map help
```

### known issues
- any moving or variable entrance/exit. (the door, truck, horse, nexus, etc etc)

### using the map

- Load the map:
```
rm
^^ actually just runs the following:
#map read $dir/maps/eotl.map

```

- Start the map in the correct room e.g. the "Lounge":
```
#map goto 1
```

- Check the list of rooms (a bunch don't have names yet sorry):
```
#map list
```

- Run to a room:
```
#map run 3
```
OR
```
#map run {Lounge}
```
- Checkout the cool console based MAP!!!!
```
> #map map
                                      |                 |                       |                             |                             |                       |                 |
                                     [ ]               [ ]                     [ ]                           [ ]                           [ ]                     [ ]               [ ]
                                      |                 |                       |                             |                             |                       |                 |
                                      |                 |                       |                             |                             |                       |                 |
                                     [ ]               [ ]                     [ ]                           [ ]                           [ ]                     [ ]---[ ]         [ ]
                                      |                 |                       |                             |                             |                       |     |           |
                                      |                 |                       |                             |                             |                       |     |           |   
             [ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]--
              |                       |                 |                       |                             |                             |                       |                 |   
              |                       |                 |                       |                             |                             |                       |                 |
             [ ]                     [ ]               [ ]                     [ ]                           [ ]                           [ ]                     [ ]               [ ]
              |                       |                 |                       |                             |                             |                       |                 |
              |                       |                 |                       |                             |                             |                       |                 |
             [ ]                     [ ]               [ ]                     [ ]                           [ ]---[ ]                     [ ]                     [ ]               [ ]
              |                       |                 |                       |                             |     |                       |                       |                 |
              |                       |                 |                       |                             |     |                       |                       |                 |
             [ ]                     [ ]               [ ]                     [ ]                     [ ]---[ ]---[ ]---[ ]               [ ]                     [ ]               [ ]
              |                       |                 |                       |                       |     |     |     |                 |                       |                 |
              |                       |                 |                       |                       |     |     |     |                 |                       |                 |
       [ ]---[ ]---[ ]   [ ]         [ ]               [ ]                     [ ]               [ ]---[ ]---[ ]---[ ]---[ ]---[ ]         [ ]                     [ ]               [ ]
        | \ / | \ / |     |           |                 |                       |                 |     |           |     |     |           |                       |                 |
        | / \ | / \ |     |           |                 |                       |                 |     |           |     |     |           |                       |                 |   
-[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]         [ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]--
        | \ / | \ / |                 |     |     |     |                       |                 |     |           |     |           |     |                       |                 |   
        | / \ | / \ |                 |     |     |     |                       |                 |+    |           |     |           |     |                       |                 |
       [ ]---[ ]---[ ]               [ ]---[ ]---[ ]   [ ]                     [ ]               [ ]---[ ]---[ ]---[ ]---[ ]         [ ]---[ ]                     [ ]               [ ]
              |                       |     |     |     |                       |                 |     |     |     |     |                 |                       |                 |
              |                       |     |     |     |                       |                 |     |     |     |     |                 |                       |                 |
             [ ]                     [ ]---[ ]---[ ]   [ ]                     [ ]               [#]---[ ]   [ ]---[ ]---[ ]               [ ]                     [ ]               [ ]
              |                       |     |     |     |                       |                             |                             |                       |                 |
              |                       |     |     |     |                       |                             |                             |                       |                 |
             [ ]                     [ ]---[ ]---[ ]   [ ]                     [ ]                           [ ]                           [ ]                     [ ]               [ ]
              |                       |     |     |     |                       |                             |                             |                       |                 |
              |                       |     |     |     |                       |                             |                             |                       |                 |
             [ ]                     [ ]   [ ]---[ ]   [ ]                     [ ]                           [ ]                           [ ]                     [ ]               [ ]
              |                       |                 |                       |                             |                             |                       |                 |
              |                       |                 |                       |                             |                             |                       |                 |   
             [ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]--
              |                       |                 |                       |                             |                             |                       |                 |     |
              |                       |                 |                       |                             |                             |                       |                 |     |
             [ ]                     [ ]               [ ]                     [ ]                           [ ]                           [ ]                     [ ]               [ ]---[ ]
              |                       |                 |                       |                             |                             |                       |                 |   
              |                       |                 |                       |                             |                             |                       |                 |
             [ ]                     [ ]               [ ]                     [ ]                           [ ]                           [ ]                     [ ]               [ ]
              |                       |                 |                       |                             |                             |                       |                 |
              |                       |                 |                       |                             |                             |                       |                 |
             [ ]                     [ ]               [ ]                     [ ]                           [ ]                           [ ]                     [ ]               [ ]
              |                       |                 |                       |                             |                             |                       |                 |
              |                       |                 |                       |                             |                             |                       |                 |
             [ ]                     [ ]               [ ]                     [ ]                           [ ]                           [ ]                     [ ]               [ ]
              |                       |                 |                       |                             |                             |                       |                 |
              |                       |                 |                       |                             |                             |                       |                 |
             [ ]                     [ ]               [ ]                     [ ]                           [ ]                           [ ]                     [ ]               [ ]
              |                       |                 |                       |                             |                             |                       |                 |
              |                       |                 |                       |                             |                             |                       |                 |
             [ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]---[ ]
                                      |                 |           |           |                             |                             |                       |                 |
```

### checkout all the mapped runs
```
#alias
#grep run
```


