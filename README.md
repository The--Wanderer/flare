## FAQ

### What is flare?

Flare is a project oriented towards creating a uniform standard with Runescape private emulation.

## Frame Standards

### Menu Options

All subjects have up to 5 options. Their frame id is sequential from the one listed in the table.

__Example: Ground item options start at x so therefore the frame id for each option will be (x + optionid)__

#### Item Options

_CHECK THIS FOR CONSISTENCY WITH 3xx-400_

```

 Frames                   Structure

 +-----+---------------------+    +--------------+----------------+--------------------+
 | ID  | Name                |    | uint_16 : id | uint_16 : slot | int_32 : widgetid  |
 +-----+---------------------+    +--------------+----------------+--------------------+
 | NA  | Interaction Options |
 +-----+---------------------+
 | NA  | Widget Options      |
 +-----+---------------------+
```

#### Mobile Entity Options

```

 Frames                   Structure
 
 +-----+-------------+    +--------------+
 | ID  | Entity Name |    | uint_16 : id |
 +-----+-------------+    +--------------+
 | NA  | Player      |
 +-----+-------------+
 | NA  | NPC         |
 +-----+-------------+
```

#### Still Entity Options

```

 Frames                    Structure

 +-----+--------------+    +--------------+----------------+----------------+
 | ID  | Entity Name  |    | uint_16 : id | uint_16 : posx | uint_16 : posy |
 +-----+--------------+    +--------------+----------------+----------------+
 | NA  | Ground Item  |
 +-----+--------------+
 | NA  | Still Object |
 +-----+--------------+
```

### Social List Updates


```

 Frames                     Structure

 +-----+---------------+    +----------------+
 | ID  | Name          |    | int_64 : name  |
 +-----+---------------+    +----------------+
 | NA  | Friend Add    |
 +-----+---------------+
 | NA  | Friend Remove |
 +-----+---------------+
 | NA  | Ignore Add    |
 +-----+---------------+
 | NA  | Ignore Remove |
 +-----+---------------+
```