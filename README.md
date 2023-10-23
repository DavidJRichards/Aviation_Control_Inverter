# Aviation_Control_Inverter
### Ferranti Control Inverter Box, Type E 

 * Output 115V 400Hz

## Markings

 * ST.REF.No. 6A/6846
 * SerNo 804/64
 * (Alt) 6A/105831
 * INST/A471
 * INST/A660
 * UFI

## Appearance
![overview](./images/IMG_20231005_200845.jpg) 

### [images](./images/README.md)

## DC Input 

|         |           |  |
|---------|-----------|--|
| +A      | +ve 26 VDC|1-3-0|
|         |           |2-0-4|
|         |           |     |
| -B      | 0v        |1-4-2|
|         |           |2-0-3|
|         |           |     |
| Chassis |           |2-0-6|
|         |           |2-0-5|
|         |           |1-5-9|

 * When DC is applied approx 1/2 amp is drawn from DC supply with no additional AC load

## 12 pin connector, ART.HORIZON
![connector](./images/IMG_20231007_094204_small.jpg)

|   |          |                             |     |
|---|----------|-----------------------------|-----|
| A |Rly-3-1   |gen sw AC out - 68 ohms to B-|2-0-1|
| B |B-        |Common negative, chassis     |2-0-2|
| C |Inductor  |ind AC out - 31 ohms to A    |1-6-0|
| D |Rly-2-8   |AC out switched              |1-5-2|
| E |Rly-2-4   |AC out switched              |1-5-1|
| F |Rly-3-5   |sw relay out                 |1-4-9|
| H |Rly-1-1   |H-J switched-a  (B-)         |1-5-5|
| J |Rly-1-3   |H-J switched-b               |1-3-6|
| K |Rly-1-7   |K-N switched-a               |1-3-7|
| L |Rly-4-8   |switched DC                  |1-4-8|
| M |Rly123-Pve|Relay energise input         |1-5-6|
| N |Rly-1-5   |K-N switched-b               |1-5-3|


## Output Transformer

[transformer](./images/IMG_20231005_214843.jpg)

[transformer-pins](./images/IMG_20231007_103241.jpg)

|   |       |                    |
|---|-------|--------------------|
| 1 | n/c   |                    |
| 2 | tr2-e | 1-0-8              |
| 3 | B-    | 1-1-8, 1-1-7       |
| 4 | B-    | 1-1-6, 1-1-7, 1-0-1|
| 5 | n/c   |                    |
| 6 | n/c   |                    |
| 7 | sw +ve| 1-1-0, 1-2-2       |
| 8 | n/c   |                    |
| 9 | tr1-e | 1-0-4              |
|10 | gen AC| 1-1-9              |
|11 | B-    | 1-2-0, 1-1-8, 1-2-1|

 * small capacitor on transformer pins 7 to 11

## transistor capacitor

| | |
|-|-|
|-ve|1-0-1, 1-0-2|
|+ve|1-4-1|

## transistor-1

|     |              |
|-----|--------------|
|  b  | 1-0-3        |
|  e  | 1-0-4        |
|  c  | 1-0-5, 1-4-0 |

## transistor-2

|     |             |
|-----|-------------|
|   b | 1-0-7       |
|   e | 1-0-8       |
|   c | 1-0-6, 1-4-0|



## Inductor output

|       |     |
|-------|-----|
| C     |     |
| 1-2-5 |     |
| 1-6-0 |     |
|       |     |
| A     |     |
| 1-2-3 |     |
| 1-2-4 |     |

## Capacitor output

|       |     |
|-------|-----|
| A     |     |
| 1-5-0 |     |
| 2-0-1 |     |
|       |     |
| B     |     |
| 1-5-5 |     |
| 2-0-2 |     |



## Relays

 * 26 Volt,  618 Ohm,  DPCO

[Relays](./images/IMG_20231007_103348.jpg)

 * rly4 - rly3 - rly2 -rly1

[Relay](./images/Relay.jpg) [Relay](./images/RelayPins.jpg)

### pin numbering

 * 10 is AC transformer output, gen AC
 * Letters are output connector terminals
 * 1-2_9 is wire identification number

|    |    |       | |
|----|----|-------|-|
| 1-1|ncl | H     |1-5-4|H-J switched-a |
| 1-3|com | J     |1-5-8|H-J switched-b |
| 1-8|nop | n/c   |
|    |    |       |
| 1-5|ncl | N     |1-5-3|K-N switched-b |
| 1-7|com | K     |1-5-7|K-N switched-a |
| 1-4|nop | n/c   |
|    |    |       |
| 1-2|coil|       |1-5-5|Relay common ip|
| 1-6|coil|       |1-5-6, 1-6-1|Relay energise ip|
|    |    |       |
| 2-1|ncl | n/c   |
| 2-3|com | 10    |1-6-8, 1-6-9|gen AC|
| 2-8|nop | D     |1-9-2|
|    |    |       |
| 2-5|ncl | n/c   |
| 2-7|com | 10    |1-6-9|gen AC|
| 2-4|nop | E     |1-5-1|
|    |    |       |
| 2-2|coil|       |1-6-4, 1-6-5|Relay common ip|
| 2-6|coil|       |1-6-6, 1-6-7|Relay energise ip|
|    |    |       |
| 3-1|ncl | A     |1-5-0, 1-2-3|
| 3-3|com | 10    |1-1-9, 1-6-8|gen AC|
| 3-8|nop | n/c   |
|    |    |       |
| 3-5|ncl |  F    |1-4-9|sw relay out   |
| 3-7|com | sw +ve|1-2-2|
| 3-4|nop | n/c   |
|    |    |       |
| 3-2|coil|       |1-6-4|Relay common ip|
| 3-6|coil|       |1-6-6|Relay energise ip|
|    |    |       |
|    |    |       |
| 4-1|ncl | n/c   |
| 4-3|com | ?     |1-2-9|diode DC+      |
| 4-8|nop | L     |1-4-8|switched DC    |
|    |    |       |
| 4-5|ncl | n/c   |
| 4-7|com | n/c   |
| 4-4|nop | n/c   |
|    |    |       |
| 4-2|coil| B-    |1-6-3, 1-4-3|
| 4-6|coil|       |1-2-7|Relay4 energise|
|    |    |       |


 * Relay 4 is activated when main DC power is applied
 * Relays 1,2,3 coils are wired in parallel and activated when +ve applied to input M

## Button capacitor

|     |                   |
|-----|-------------------|
|  -  |1-0-1, 1-4-2, 1-4-3|
|  +  |1-0-9, 1-2-8       |


|                |            |
|----------------|------------|
|c 11            |1-2-1       |
|c red,d red,r   |1-2-6, 1-2-7| relay4 energise|
|r               |1-1-1|
|d yellow, sw +ve|1-1-0|


## Diode

|         | |
|---------|-|
|+ve DC in|1-3-0              |
|diode DC+|1-2-8, 1-2-9, 1-0-6|

## capacitors

|       |            |
|-------|------------|
|A+     |2-0-4       |
|Chassis|2-0-5       |
|       |            |
|B-     |2-0-3       |
|Chassis|2-0-6       |
|       |            |
|Chassis|1-5-9       |
|       |            |
|B-     |1-5-5, 2-0-2|
|       |1-5-0, 2-0-1|
|       |            |


## internal wiring

|       |        |         |
|-------|--------|---------|
|  1-2-9| rly4-3 |diode DC+|
