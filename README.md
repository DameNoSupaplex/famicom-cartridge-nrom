# famicom-cartridge-nrom

NROM famicom cartridge board with 32Kb PRG and 8Kb CHR 

## famicom pinout
```
             ┌───────┐
      GND -- │01   31│ -- +5V
  CPU A11 -> │02   32│ <- M2
  CPU A10 -> │03   33│ <- CPU A12
   CPU A9 -> │04   34│ <- CPU A13
   CPU A8 -> │05   35│ <- CPU A14
   CPU A7 -> │06   36│ <> CPU D7
   CPU A6 -> │07   37│ <> CPU D6
   CPU A5 -> │08   38│ <> CPU D5
   CPU A4 -> │09   39│ <> CPU D4
   CPU A3 -> │10   40│ <> CPU D3
   CPU A2 -> │11   41│ <> CPU D2
   CPU A1 -> │12   42│ <> CPU D1
   CPU A0 -> │13   43│ <> CPU D0
  CPU R/W -> │14   44│ <- /ROMSEL (/A15 + /M2)
     /IRQ <- │15   45│ <- Audio from 2A03
      GND -- │16   46│ -> Audio to RF
  PPU /RD -> │17   47│ <- PPU /WR
CIRAM A10 <- │18   48│ -> CIRAM /CE
   PPU A6 -> │19   49│ <- PPU /A13
   PPU A5 -> │20   50│ <- PPU A7
   PPU A4 -> │21   51│ <- PPU A8
   PPU A3 -> │22   52│ <- PPU A9
   PPU A2 -> │23   53│ <- PPU A10
   PPU A1 -> │24   54│ <- PPU A11
   PPU A0 -> │25   55│ <- PPU A12
   PPU D0 <> │26   56│ <- PPU A13
   PPU D1 <> │27   57│ <> PPU D7
   PPU D2 <> │28   58│ <> PPU D6
   PPU D3 <> │29   59│ <> PPU D5
      +5V -- │30   60│ <> PPU D4
             └───────┘
```

## M27C256B pinout
```
    ┌────┬───┬────┐
Vpp ┤01  └───┘  28├ Vcc
A12 ┤02         27├ A14
 A7 ┤03         26├ A13
 A6 ┤04         25├ A8
 A5 ┤05         24├ A9
 A4 ┤06         23├ A11
 A3 ┤07         22├ /G
 A2 ┤08         21├ A10
 A1 ┤09         20├ /E
 A0 ┤10         19├ Q7
 Q0 ┤11         18├ Q6
 Q1 ┤12         17├ Q5
 Q2 ┤13         16├ Q4
Vss ┤14         15├ Q3
    └─────────────┘
```

## M27C64A pinout
```
    ┌────┬───┬────┐
Vpp ┤01  └───┘  28├ Vcc
A12 ┤02         27├ /P
 A7 ┤03         26├ NC
 A6 ┤04         25├ A8
 A5 ┤05         24├ A9
 A4 ┤06         23├ A11
 A3 ┤07         22├ /G
 A2 ┤08         21├ A10
 A1 ┤09         20├ /E
 A0 ┤10         19├ Q7
 Q0 ┤11         18├ Q6
 Q1 ┤12         17├ Q5
 Q2 ┤13         16├ Q4
Vss ┤14         15├ Q3
    └─────────────┘
```