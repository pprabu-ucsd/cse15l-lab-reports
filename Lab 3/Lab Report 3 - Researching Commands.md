# Lab Report 3 - Researching Commands

**By Pranav Prabu**

> For this lab, I will be researching the functions of the `less` command.

## Option 1: -N

Format:

`$ less -N <file-path>`

This option in the `less` command shows line numbers at the side of the opened file. This option is useful, as it would be helpful for any user looking to cite a specific piece of evidence by using the line numbers on the right as a guide.

Example 1:

`$ less -N ./written_2/travel_guides/berlitz1/HistoryEdinburgh.txt`

Result:
```
      1 
      2   
      3   
      4     
      5       
      6         A Brief History
      7         The city of Edinburgh grew up around the steep, ragged cliff
      8         of the Castle Rock and its easily defended summit. Archaeological
      9         excavations have revealed evidence of habitation here as long ago as
     10         900 b.c. Very little, however, is known about the Rock and its
     11         inhabitants in the centuries between its first occupation and the time
     12         of the MacAlpin kings. A few shadowy details have been left to us by
     13         the Romans and by an epic poem from the seventh century.
     14         Romans and Britons
     15         The Romans invaded Scotland in a.d. 78<E2><80><93>84, where they met a
     16         fierce group called the Picts, whom they drove north. They consolidated
:
```

> Line numbers show up on the left

Example 2:

`$ less -N ./written_2/travel_guides/berlitz2/California-WhereToGo.txt`

Result:
```
      1 
      2 
      3 
      4 
      5 Where to Go
      6 Many Californians would like to divide their state into two new states, Northern and Southern California<C2><A0><E2><80><94><C2><A0>corresponding to what they believe to be two di
      6 stinct frames of mind as represented by San Francisco and Los Angeles. In fact you will find a little bit of both<C2><A0><E2><80><94><C2><A0>San Francisco<E2><80><99>s sophisticat
      6 ion and Los Angeles<E2><80><99> sunny craziness<C2><A0><E2><80><94><C2><A0>all over the place.
      7 Our journey begins with San Francisco and its nearby attractions and works its way down the coast to Los Angeles and San Diego before heading inland to the mountains and deserts o      7 f the Sierra Nevada and Death Valley. You can turn this itinerary upside down if you prefer, but either way, you should also consider making an excursion to Las Vegas, California
      7 <E2><80><99>s favorite out-of-state playground.
      8 You can get to almost all these places by train or bus, and air travel is quite cheap. However, the car is king, and it<E2><80><99>s difficult to enjoy the full scope of this vast      8  and varied landscape without driving. San Francisco is unusual for California in that it is a walker<E2><80><99>s town, with buses and cable cars to help you up and down the hill      8 s. Los Angeles is undeniably car country, though it is trying to alleviate its congestion and pollution by building a light-rail network. Out-of-town attractions such as the natio      8 nal parks, and especially Death Valley, are most easily reached by car, although once there it<E2><80><99>s more rewarding to leave your vehicle behind and explore on foot.
      9 San Francisco
:
```

> Line numbers show up on the left

## Option 2: -X

Format:

`$ less -X <file-path>`

This option in the `less` command keeps the file open in the terminal even after finishing the command. This option is useful, as after using this option, you do not have to continually open up the file again using `less`, and simply have it in the terminal even after ending the command.

Example 1:

`$ less -X ./written_2/travel_guides/berlitz1/HistoryEdinburgh.txt`

Result:
```
[cs15lwi23aaw@ieng6-202]:skill-demo1-data:203$ less -X ./written_2/travel_guides/berlitz1/HistoryEdinburgh.txt

  
  
    
      
        A Brief History
        The city of Edinburgh grew up around the steep, ragged cliff
        of the Castle Rock and its easily defended summit. Archaeological
        excavations have revealed evidence of habitation here as long ago as
        900 b.c. Very little, however, is known about the Rock and its
        inhabitants in the centuries between its first occupation and the time
        of the MacAlpin kings. A few shadowy details have been left to us by
        the Romans and by an epic poem from the seventh century.
        Romans and Britons
        The Romans invaded Scotland in a.d. 78<E2><80><93>84, where they met a
        fierce group called the Picts, whom they drove north. They consolidated
[cs15lwi23aaw@ieng6-202]:skill-demo1-data:203$
```

> The file is left open in the terminal even after ending the command

Example 2:

`$ less -X ./written_2/travel_guides/berlitz2/California-WhereToGo.txt`

Result:
```
[cs15lwi23aaw@ieng6-202]:skill-demo1-data:203$ less -X ./written_2/travel_guides/berlitz2/California-WhereToGo.txt
"./written_2/travel_guides/berlitz2/California-WhereToGo.txt" may be a binary file.  See it anyway? 




        Where to Go 
        Many Californians would like to divide their state into two new states, Northern and Southern California<C2><A0><E2><80><94><C2><A0>corresponding to what they believe to be two distinct frames of mind as represented by San Francisco and Los Angeles. In fact you will find a little bit of both<C2><A0><E2><80><94><C2><A0>San Francisco<E2><80><99>s sophistication and Los Angeles<E2><80><99> sunny craziness<C2><A0><E2><80><94><C2><A0>all over the place.
        Our journey begins with San Francisco and its nearby attractions and works its way down the coast to Los Angeles and San Diego before heading inland to the mountains and deserts of the Sierra Nevada and Death Valley. You can turn this itinerary upside down if you prefer, but either way, you should also consider making an excursion to Las Vegas, California<E2><80><99>s favorite out-of-state playground.
        You can get to almost all these places by train or bus, and air travel is quite cheap. However, the car is king, and it<E2><80><99>s difficult to enjoy the full scope of this vast and varied landscape without driving. San Francisco is unusual for California in that it is a walker<E2><80><99>s town, with buses and cable cars to help you up and down the hills. Los Angeles is undeniably car country, though it is trying to alleviate its congestion and pollution by building a light-rail network. Out-of-town attractions such as the national parks, and especially Death Valley, are most easily reached by car, although once there it<E2><80><99>s more rewarding to leave your vehicle behind and explore on foot.
        San Francisco
[cs15lwi23aaw@ieng6-202]:skill-demo1-data:204$ 
```

> The file is left open in the terminal even after ending the command

## Option 3: -p

Format:

`$ less -p<pattern> <file-path>`

This option in the `less` command highlights all matches within the file with the given pattern (is case-sensitive). This option is helpful, as if you are looking for a specfic piece of evidence within a text or file, using this option, you lessen the time spent searching for the specific piece of evidence needed.

Example 1:

`$ less -pthe ./written_2/travel_guides/berlitz1/HistoryEdinburgh.txt`

Result:
```
        A Brief History
        The city of Edinburgh grew up around ==the== steep, ragged cliff
        of ==the== Castle Rock and its easily defended summit. Archaeological
        excavations have revealed evidence of habitation here as long ago as
        900 b.c. Very little, however, is known about ==the== Rock and its
        inhabitants in ==the== centuries between its first occupation and ==the== time
        of ==the== MacAlpin kings. A few shadowy details have been left to us by
        ==the== Romans and by an epic poem from ==the== seventh century.
        Romans and Britons
        The Romans invaded Scotland in a.d. 78<E2><80><93>84, where ==the==y met a
        fierce group called ==the== Picts, whom ==the==y drove north. They consolidated
        ==the==ir gains by building Antonine<E2><80><99>s Wall across ==the== waist of Scotland
        between ==the== Firth of Forth and ==the== River Clyde in about a.d. 150.
        Roman legions encountered ==the== strongholds of ==the== Castle Rock
        and Arthur<E2><80><99>s Seat, held by a tribe of ancient Britons known as ==the==
        Votadini. Little is recorded about this group, but ==the==y were probably
:
```

> The highlighted text matches with the pattern given in the command

Example 2:

`$ less -pthe ./written_2/travel_guides/berlitz2/California-WhereToGo.txt`

Result:
```
        Where to Go
        Many Californians would like to divide ==the==ir state into two new states, Nor==the==rn and Sou==the==rn California<C2><A0><E2><80><94><C2><A0>corresponding to what ==the==y believe to be two distinct f
        rames of mind as represented by San Francisco and Los Angeles. In fact you will find a little bit of both<C2><A0><E2><80><94><C2><A0>San Francisco<E2><80><99>s sophistication and Los Angeles<E2><80><99> sunny craziness<C2><A0><E2><80><94><C2><A0>all over ==the== place.
        Our journey begins with San Francisco and its nearby attractions and works its way down ==the== coast to Los Angeles and San Diego before heading inland to ==the== mountains and deserts of ==the== Sierra Nevada and Death Valley. You can turn this itinerary upside down if you prefer, but ei==the==r way, you should also consider making an excursion to Las Vegas, California<E2><80><99>s favorite out-of-state playground.
        You can get to almost all ==the==se places by train or bus, and air travel is quite cheap. However, ==the== car is king, and it<E2><80><99>s difficult to enjoy ==the== full scope of this vast and varied landscape without driving. San Francisco is unusual for California in that it is a walker<E2><80><99>s town, with buses and cable cars to help you up and down ==the== hills. Los Angeles is undeniably car country, though it is trying to alleviate its congestion and pollution by building a light-rail network. Out-of-town attractions such as ==the== national parks, and especially Death Valley, are most easily reached by car, although once ==the==re it<E2><80><99>s more rewarding to leave your vehicle behind and explore on foot.
        San Francisco
        San Franciscans are quite unashamedly in love with ==the==ir town. Its natural setting, nestled in ==the== hills around ==the== bay, makes ==the== city uncommonly cozy; ==the== zip in ==the== air is invigorating
        , and even ==the== fog that rolls in off ==the== ocean seems more romantic than chilling. If you have a car, one way to begin your visit is to travel along 49-Mile Drive, which provides a compreh
        ensive tour of ==the== main sights. You<E2><80><99>ll need to use a good map, as ==the== blue signposts with a white seagull in ==the== center can be difficult to locate. Stop off at Twin Peaks (==the== 
        road to get ==the==re starts near ==the== sou==the==rn end of Market Street) for an excellent panoramic view of ==the== city and ==the== bay, ==the==n park ==the== car, put on a pair of comfortable walking shoes, an
:
```

> The highlighted text matches with the pattern given in the command

## Option 4: -m

Format:

`$ less -m <file-path>`

This option in the `less` command shows the percentage of the file read so far within the terminal. This option is helpful, as when reading parts of the opened file through the `less` command, it is hard to see how far you are into the file. This option helps to streamline the process and inform the user how far they are in the file through a concise method.

Example 1:

`$ less -m ./written_2/travel_guides/berlitz1/HistoryEdinburgh.txt`

Result:
```
        A Brief History
        The city of Edinburgh grew up around the steep, ragged cliff
        of the Castle Rock and its easily defended summit. Archaeological
        excavations have revealed evidence of habitation here as long ago as
        900 b.c. Very little, however, is known about the Rock and its
        inhabitants in the centuries between its first occupation and the time
        of the MacAlpin kings. A few shadowy details have been left to us by
        the Romans and by an epic poem from the seventh century.
        Romans and Britons
        The Romans invaded Scotland in a.d. 78<E2><80><93>84, where they met a
        fierce group called the Picts, whom they drove north. They consolidated
        their gains by building Antonine<E2><80><99>s Wall across the waist of Scotland
        between the Firth of Forth and the River Clyde in about a.d. 150.
        Roman legions encountered the strongholds of the Castle Rock
        and Arthur<E2><80><99>s Seat, held by a tribe of ancient Britons known as the
        Votadini. Little is recorded about this group, but they were probably
5%
```

> The percentage of the file read is shown at the bottom left

Example 2:

`$ less -m ./written_2/travel_guides/berlitz2/California-WhereToGo.txt`

Result:
```
        Where to Go
        Many Californians would like to divide their state into two new states, Northern and Southern California<C2><A0><E2><80><94><C2><A0>corresponding to what they believe to be two distinct frames of mind as represented by San Francisco and Los Angeles. In fact you will find a little bit of both<C2><A0><E2><80><94><C2><A0>San Francisco<E2><80><99>s sophistication and Los Angeles<E2><80><99> sunny craziness<C2><A0><E2><80><94><C2><A0>all over the place.
        Our journey begins with San Francisco and its nearby attractions and works its way down the coast to Los Angeles and San Diego before heading inland to the mountains and deserts of the Sierra Nevada and Death Valley. You can turn this itinerary upside down if you prefer, but either way, you should also consider making an excursion to Las Vegas, California<E2><80><99>s favorite out-of-state playground.
        You can get to almost all these places by train or bus, and air travel is quite cheap. However, the car is king, and it<E2><80><99>s difficult to enjoy the full scope of this vast and varied landscape without driving. San Francisco is unusual for California in that it is a walker<E2><80><99>s town, with buses and cable cars to help you up and down the hills. Los Angeles is undeniably car country, though it is trying to alleviate its congestion and pollution by building a light-rail network. Out-of-town attractions such as the national parks, and especially Death Valley, are most easily reached by car, although once there it<E2><80><99>s more rewarding to leave your vehicle behind and explore on foot.
        San Francisco
        San Franciscans are quite unashamedly in love with their town. Its natural setting, nestled in the hills around the bay, makes the city uncommonly cozy; the zip in the air is invigorating
        , and even the fog that rolls in off the ocean seems more romantic than chilling. If you have a car, one way to begin your visit is to travel along 49-Mile Drive, which provides a compreh
        ensive tour of the main sights. You<E2><80><99>ll need to use a good map, as the blue signposts with a white seagull in the center can be difficult to locate. Stop off at Twin Peaks (the 
        road to get there starts near the southern end of Market Street) for an excellent panoramic view of the city and the bay, then park the car, put on a pair of comfortable walking shoes, an3%
```

> The percentage of the file read is shown at the bottom left 

## Sources
To find all of these options for the less command, I used these two sources.

[https://linuxize.com/post/less-command-in-linux/](https://linuxize.com/post/less-command-in-linux/)

[https://phoenixnap.com/kb/less-command-in-linux#ftoc-heading-4](https://phoenixnap.com/kb/less-command-in-linux#ftoc-heading-4)
