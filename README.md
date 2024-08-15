# txt-compressor

A simple text compressor that uses the Huffman algorithm to compress and decompress text file.

this project depends on the bun runtime, you can install it from
[https://bun.sh](https://bun.sh)

```bash
curl -fsSL https://bun.sh/install | bash
```

if you have bun installed you can run the following commands to install and run the project:

```bash
bun install
```

# Usage

```bash
bun index.ts <encode|decode> <input file> [options]
```

## Options

- `-e, --encode <string>`: Specify the input file to encode.
- `-d, --decode <string>`: Specify the input file to decode.
- `-o, --outputFileName <string>`: Specify the output file name.
- `-m, --mermaid`: Enable Mermaid diagram generation for the Huffman tree.

This project was created using `bun init` in bun v1.1.18. [Bun](https://bun.sh) is a fast all-in-one JavaScript runtime.

sample of mermaid diagram:

```mermaid
graph TD;
A((3250625))
A --> B((1903787))
B --> C((1063060))
C --> D((546711))
D --> E((294387))
E --> F((149296))
F --> G((75710))
G --> H["y 37944"]
G --> I((37766))
I --> J((19783))
J --> K((9999))
K --> L((5044))
L --> M((2530))
M --> N((1291))
N --> O((661))
O --> P["X 333"]
O --> Q((328))
Q --> R["] 164"]
Q --> S["[ 164"]
N --> T((630))
T --> U["K 320"]
T --> V((310))
V --> W["4 160"]
V --> X((150))
X --> Y((76))
Y --> Z["î 39"]
Y --> AA["ü 37"]
X --> AB["ê 74"]
M --> AC["Y 1239"]
L --> AD["G 2514"]
K --> AE((4955))
AE --> AF[": 2501"]
AE --> AG["L 2454"]
J --> AH((9784))
AH --> AI["E 4939"]
AH --> AJ((4845))
AJ --> AK["J 2447"]
AJ --> AL["q 2398"]
I --> AM((17983))
AM --> AN((9291))
AN --> AO["- 4700"]
AN --> AP["C 4591"]
AM --> AQ((8692))
AQ --> AR["S 4411"]
AQ --> AS((4281))
AS --> AT["V 2211"]
AS --> AU["_ 2070"]
F --> AV["
73586"]
E --> AW["r 145091"]
D --> AX((252324))
AX --> AY((132138))
AY --> AZ["u 67391"]
AY --> BA((64747))
BA --> BB["b 34267"]
BA --> BC[". 30480"]
AX --> BD((120186))
BD --> BE["c 62741"]
BD --> BF((57445))
BF --> BG((29286))
BG --> BH((14933))
BH --> BI((7564))
BI --> BJ((3857))
BJ --> BK((2012))
BK --> BL((1102))
BL --> BM((581))
BM --> BN["è 293"]
BM --> BO((288))
BO --> BP["É 146"]
BO --> BQ["6 142"]
BL --> BR((521))
BR --> BS((270))
BS --> BT["Q 135"]
BS --> BU((135))
BU --> BV((71))
BV --> BW((36))
BW --> BX["ù 18"]
BW --> BY["ï 18"]
BV --> BZ["œ 35"]
BU --> CA((64))
CA --> CB["ô 34"]
CA --> CC((30))
CC --> CD((17))
CD --> CE((9))
CE --> CF["ë 5"]
CE --> CG((4))
CG --> CH((2))
CH --> CI["& 1"]
CH --> CJ["# 1"]
CG --> CK((2))
CK --> CL["{ 1"]
CK --> CM["½ 1"]
CD --> CN((8))
CN --> CO((4))
CO --> CP["ñ 2"]
CO --> CQ["Ü 2"]
CN --> CR((4))
CR --> CS["$ 2"]
CR --> CT["Ç 2"]
CC --> CU((13))
CU --> CV["' 7"]
CU --> CW["/ 6"]
BR --> CX((251))
CX --> CY["7 132"]
CX --> CZ((119))
CZ --> DA["Z 60"]
CZ --> DB["à 59"]
BK --> DC((910))
DC --> DD((466))
DD --> DE["3 239"]
DD --> DF["2 227"]
DC --> DG((444))
DG --> DH["‘ 224"]
DG --> DI((220))
DI --> DJ["9 114"]
DI --> DK["æ 106"]
BJ --> DL["z 1845"]
BI --> DM["’ 3707"]
BH --> DN["A 7369"]
BG --> DO((14353))
DO --> DP((7234))
DP --> DQ["x 3693"]
DP --> DR["R 3541"]
DO --> DS["“ 7119"]
BF --> DT((28159))
DT --> DU["k 14107"]
DT --> DV((14052))
DV --> DW["” 7048"]
DV --> DX((7004))
DX --> DY["! 3539"]
DX --> DZ((3465))
DZ --> EA["D 1758"]
DZ --> EB((1707))
EB --> EC["U 904"]
EB --> ED((803))
ED --> EE["8 404"]
ED --> EF((399))
EF --> EG["0 205"]
EF --> EH((194))
EH --> EI((105))
EI --> EJ["â 56"]
EI --> EK((49))
EK --> EL["| 27"]
EK --> EM[""" 22"]
EH --> EN((89))
EN --> EO["ç 48"]
EN --> EP((41))
EP --> EQ((22))
EQ --> ER((12))
ER --> ES["È 6"]
ER --> ET((6))
ET --> EU["Œ 3"]
ET --> EV((3))
EV --> EW((2))
EW --> EX["… 1"]
EW --> EY["} 1"]
EV --> EZ["% 1"]
EQ --> FA["Æ 10"]
EP --> FB((19))
FB --> FC((10))
FC --> FD["+ 5"]
FC --> FE["À 5"]
FB --> FF["û 9"]
C --> FG[" 516349"]
B --> FH((840727))
FH --> FI((439387))
FI --> FJ["t 223000"]
FI --> FK((216387))
FK --> FL((109421))
FL --> FM["m 56000"]
FL --> FN["f 53421"]
FK --> FO["d 106966"]
FH --> FP((401340))
FP --> FQ((201608))
FQ --> FR((104495))
FR --> FS["w 53330"]
FR --> FT((51165))
FT --> FU((26346))
FU --> FV((13440))
FV --> FW((6837))
FW --> FX["P 3426"]
FW --> FY["O 3411"]
FV --> FZ["H 6603"]
FU --> GA((12906))
GA --> GB((6585))
GB --> GC["j 3391"]
GB --> GD["B 3194"]
GA --> GE((6321))
GE --> GF["W 3177"]
GE --> GG["— 3144"]
FT --> GH((24819))
GH --> GI["T 12571"]
GH --> GJ((12248))
GJ --> GK["M 6212"]
GJ --> GL((6036))
GL --> GM["N 3060"]
GL --> GN["? 2976"]
FQ --> GO["l 97113"]
FP --> GP["a 199732"]
A --> GQ((1346838))
GQ --> GR((698331))
GR --> GS((361249))
GS --> GT["o 180974"]
GS --> GU((180275))
GU --> GV((94809))
GV --> GW[", 48780"]
GV --> GX["g 46029"]
GU --> GY((85466))
GY --> GZ((45526))
GZ --> HA["v 24047"]
GZ --> HB((21479))
HB --> HC((11370))
HC --> HD["; 5885"]
HC --> HE((5485))
HE --> HF["F 2766"]
HE --> HG((2719))
HG --> HH((1392))
HH --> HI((699))
HI --> HJ((360))
HJ --> HK["5 190"]
HJ --> HL[") 170"]
HI --> HM((339))
HM --> HN["( 170"]
HM --> HO["* 169"]
HH --> HP["1 693"]
HG --> HQ["é 1327"]
HB --> HR["I 10109"]
GY --> HS["p 39940"]
GR --> HT((337082))
HT --> HU["h 170220"]
HT --> HV["n 166862"]
GQ --> HW((648507))
HW --> HX["e 325664"]
HW --> HY((322843))
HY --> HZ["i 165211"]
HY --> IA["s 157632"]
```
