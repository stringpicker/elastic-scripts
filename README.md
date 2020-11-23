# elastic-scripts
Some useful scripts for monitoring and managing Elasticsearch clusters

Usage:
```
esHealthCheck.py [-h] [--username USERNAME] [--password PASSWORD] [--version]
```

Sample results:
```
--------------
Company-CCS-US
--------------
Getting cluster health info for Company-CCS-US... 
Getting cluster settings for Company-CCS-US... 
Getting cluster stats for Company-CCS-US... 
Enumerating nodes in cluster Company-CCS-US...
Getting cluster health info for node QTHoC1HBSC3jshCOOmcgqNFl7w... 
Getting cluster health info for node sPR5gajsSd22adzLd-G5eerpqw... 
Getting cluster health info for node cTONas2skGzdSR2xSSeZ31qF5Q... 
Getting cluster health info for node RJ9wjOhPRzCnbyBedsa3yk_kGQ... 
--------------
Company-CCS-UK
--------------
Getting cluster health info for Company-CCS-UK... 
Getting cluster settings for Company-CCS-UK... 
Getting cluster stats for Company-CCS-UK... 
Enumerating nodes in cluster Company-CCS-UK...
Getting cluster health info for node q83jFtGSQFujnUtsdxzjdEtUyQ... 
Getting cluster health info for node E0h3c5pURQmMvcsdw2R9S6Q-Dg... 
Getting cluster health info for node PZmABkLbTbm_TOaxq3Xd4QWZwA... 
Getting cluster health info for node pDKGaWYXTFGJ6CXXasdaNY9qTg... 
--------------
Company-US1
--------------
Getting cluster health info for Company-US1... 
Getting cluster settings for Company-US1... 
Getting cluster stats for Company-US1... 
Enumerating nodes in cluster Company-US1...
Getting cluster health info for node BVMAFyXnTEiNyqssdxaJuXE7Iw... 
Getting cluster health info for node ivEq2EXbRCKpA-FasdxJChyBxg... 
Getting cluster health info for node iKUF9FQ0QAasZZasdx9jBXiqTw... 
Getting cluster health info for node ropdgqM6aswfTge37xVHs6dJhw... 
Getting cluster health info for node cM7kSY6ZT8Sjg9vaasn2Df5WuQ... 
--------------
Company-US2
--------------
Getting cluster health info for Company-US2... 
Getting cluster settings for Company-US2... 
Getting cluster stats for Company-US2... 
Enumerating nodes in cluster Company-US2...
Getting cluster health info for node b2Iq5zcKQQezYUPesd27uHKaqg... 
Getting cluster health info for node SsN7jRaVGQVGvBVqnzxcnDWyhQ... 
Getting cluster health info for node sNDyhL2nSQSQrabPXsasdwTOFQ... 
Getting cluster health info for node lfQ7I-ZxTa1GhuK-Gcxz_XMJOg... 
Getting cluster health info for node BzESJnc7RoSvX9OGTfsdawdnOA... 
--------------
Company-UK1
--------------
Getting cluster health info for Company-UK1... 
Getting cluster settings for Company-UK1... 
Getting cluster stats for Company-UK1... 
Enumerating nodes in cluster Company-UK1...
Getting cluster health info for node D7gSsgFsSQ26adas0FNcZ1Hfnw... 
Getting cluster health info for node 1uqysU4lQO2jda2adPHPSetBMQ... 
Getting cluster health info for node ojCSnYy8T9mFaasdS3GYlfdhew... 
Getting cluster health info for node amWh_xxzxznqTqeNWsseN5yrNw... 
Getting cluster health info for node NIutMCARsdawQg-ZW6jsrVgGVA... 
--------------
Company-Mon-US
--------------
Getting cluster health info for Company-Mon-US... 
Getting cluster settings for Company-Mon-US... 
Getting cluster stats for Company-Mon-US... 
Enumerating nodes in cluster Company-Mon-US...
Getting cluster health info for node nHU3MwMESSasdaiveR_IZIEVSA... 
Getting cluster health info for node hXDO8P4eSumv2asdsaTM343ZVw... 
Getting cluster health info for node R07cO9zWQ3maeasdaBifQymUbQ... 
--------------
Company-Mon-UK
--------------
Getting cluster health info for Company-Mon-UK... 
Getting cluster settings for Company-Mon-UK... 
Getting cluster stats for Company-Mon-UK... 
Enumerating nodes in cluster Company-Mon-UK...
Getting cluster health info for node D3J8zWPfSiKFM3sggIjlqA... 
╒════════════════╤══════════╤══════════╤══════════════╤═══════════════╤═════════╤═════════════╤═════════╤═══════════╤═══════════╤═══════════╤══════════════╤═══════════╕
│ display_name   │ status   │   active │   unassigned │ auto_create   │   index │         doc │    node │       jvm │ jvm       │       jvm │   processors │       mem │
│                │          │   shards │       shards │ index         │   count │       count │   count │   max(gb) │ used(%)   │   threads │              │   used(%) │
╞════════════════╪══════════╪══════════╪══════════════╪═══════════════╪═════════╪═════════════╪═════════╪═══════════╪═══════════╪═══════════╪══════════════╪═══════════╡
│ Company-CCS-US │ green    │      226 │            0 │ true          │     113 │    47474850 │       4 │      10.6 │ 48%       │       264 │            9 │        86 │
├────────────────┼──────────┼──────────┼──────────────┼───────────────┼─────────┼─────────────┼─────────┼───────────┼───────────┼───────────┼──────────────┼───────────┤
│ Company-CCS-UK │ green    │      156 │            0 │ true          │      78 │     1312081 │       4 │       3.6 │ 62%       │       253 │            8 │        69 │
├────────────────┼──────────┼──────────┼──────────────┼───────────────┼─────────┼─────────────┼─────────┼───────────┼───────────┼───────────┼──────────────┼───────────┤
│ Company-US1    │ green    │     2336 │            0 │ +.*           │    1168 │ 10108395829 │       5 │     101.5 │ 48%       │       794 │           35 │        90 │
├────────────────┼──────────┼──────────┼──────────────┼───────────────┼─────────┼─────────────┼─────────┼───────────┼───────────┼───────────┼──────────────┼───────────┤
│ Company-US2    │ green    │      310 │            0 │ +.*           │     153 │  2387197969 │       5 │      37.5 │ 45%       │       369 │           15 │        94 │
├────────────────┼──────────┼──────────┼──────────────┼───────────────┼─────────┼─────────────┼─────────┼───────────┼───────────┼───────────┼──────────────┼───────────┤
│ Company-UK1    │ green    │      780 │            0 │ +.*           │     390 │   609435467 │       5 │      10   │ 43%       │       515 │           10 │       100 │
├────────────────┼──────────┼──────────┼──────────────┼───────────────┼─────────┼─────────────┼─────────┼───────────┼───────────┼───────────┼──────────────┼───────────┤
│ Company-Mon-US │ green    │      116 │            0 │ true          │      59 │    92608271 │       3 │       4.6 │ 34%       │       178 │            6 │        93 │
├────────────────┼──────────┼──────────┼──────────────┼───────────────┼─────────┼─────────────┼─────────┼───────────┼───────────┼───────────┼──────────────┼───────────┤
│ Company-Mon-UK │ yellow   │       58 │            7 │ true          │      58 │   146515848 │       1 │       1   │ 51%       │       121 │            2 │       100 │
╘════════════════╧══════════╧══════════╧══════════════╧═══════════════╧═════════╧═════════════╧═════════╧═══════════╧═══════════╧═══════════╧══════════════╧═══════════╛
╒════════════════╤═══════════════════════╤════════════════╤════════════╤════════════╤════════════╤════════════╤═══════════╤════════════╕
│ cluster        │ server                │ host           │   rejected │   rejected │   rejected │   rejected │       jvm │        jvm │
│ alias          │ name                  │                │    refresh │     search │    watcher │      write │      heap │       heap │
│                │                       │                │    threads │    threads │    threads │    threads │   used(%) │   size(gb) │
╞════════════════╪═══════════════════════╪════════════════╪════════════╪════════════╪════════════╪════════════╪═══════════╪════════════╡
│ Company-CCS-US │ instance-0000000059   │ 10.100.10.100  │          0 │          0 │          0 │          0 │        40 │        2   │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-CCS-US │ instance-0000000066   │ 10.100.10.101  │          0 │          0 │          0 │          0 │        35 │        4   │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-CCS-US │ tiebreaker-0000000043 │ 10.100.10.102  │          0 │          0 │          0 │          0 │        21 │        0.6 │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-CCS-US │ instance-0000000060   │ 10.100.10.103  │          0 │          0 │          0 │          0 │        67 │        4   │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-CCS-UK │ instance-0000000031   │ 10.200.10.100  │          0 │          0 │          0 │          0 │        59 │        1   │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-CCS-UK │ instance-0000000030   │ 10.200.10.101  │          0 │          0 │          0 │          0 │        51 │        1   │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-CCS-UK │ tiebreaker-0000000029 │ 10.200.10.102  │          0 │          0 │          0 │          0 │        70 │        0.6 │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-CCS-UK │ instance-0000000028   │ 10.200.10.103  │          0 │          0 │          0 │          0 │        72 │        1   │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-US1    │ instance-0000000140   │ 10.101.10.100  │          0 │          0 │          0 │          0 │        30 │       14.5 │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-US1    │ instance-0000000137   │ 10.101.10.101  │          0 │          0 │          0 │          0 │        33 │       29   │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-US1    │ instance-0000000129   │ 10.101.10.102  │          0 │          0 │          0 │          0 │        28 │       14.5 │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-US1    │ instance-0000000134   │ 10.101.10.103  │          0 │          0 │          0 │         15 │        29 │       14.5 │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-US1    │ instance-0000000136   │ 10.101.10.104  │          0 │          0 │          0 │          0 │        59 │       29   │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-US2    │ instance-0000000031   │ 10.102.10.100  │          0 │          0 │          0 │          0 │        48 │        7.5 │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-US2    │ instance-0000000030   │ 10.102.10.101  │          0 │          0 │          0 │          0 │        60 │        7.5 │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-US2    │ instance-0000000036   │ 10.102.10.102  │          0 │          0 │          0 │          0 │        34 │        7.5 │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-US2    │ instance-0000000032   │ 10.102.10.103  │          0 │          0 │          0 │          0 │        62 │        7.5 │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-US2    │ instance-0000000037   │ 10.102.10.104  │          0 │          0 │          0 │          0 │        23 │        7.5 │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-UK1    │ instance-0000000072   │ 10.201.10.100  │          0 │          0 │          0 │          0 │        49 │        2   │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-UK1    │ instance-0000000069   │ 10.201.10.101  │          0 │          0 │          0 │          0 │        31 │        2   │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-UK1    │ instance-0000000068   │ 10.201.10.102  │          0 │          0 │          0 │          0 │        51 │        2   │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-UK1    │ instance-0000000070   │ 10.201.10.103  │          0 │          0 │          0 │          0 │        56 │        2   │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-UK1    │ instance-0000000071   │ 10.201.10.104  │          0 │          0 │          0 │          0 │        39 │        2   │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-Mon-US │ instance-0000000009   │ 10.103.10.100  │          0 │          0 │          0 │          0 │        39 │        2   │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-Mon-US │ tiebreaker-0000000012 │ 10.103.10.101  │          0 │          0 │          0 │          0 │        24 │        0.6 │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-Mon-US │ instance-0000000008   │ 10.203.10.100  │          0 │          0 │          0 │          0 │        30 │        2   │
├────────────────┼───────────────────────┼────────────────┼────────────┼────────────┼────────────┼────────────┼───────────┼────────────┤
│ Company-Mon-UK │ instance-0000000005   │ 10.203.10.101  │          1 │          0 │          0 │          0 │        50 │        1   │
╘════════════════╧═══════════════════════╧════════════════╧════════════╧════════════╧════════════╧════════════╧═══════════╧════════════╛
```
