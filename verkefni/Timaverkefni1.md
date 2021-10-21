## Forritað með Serial Monitor

Bjargir:
- [Skrifað í Serial Monitor](https://github.com/VESM2VT/Efni/blob/main/Kennsluefni/ArduinoForritun.md#skrifað-%C3%AD-serial-monitor)
- [Lesið frá Serial Monitor](https://github.com/VESM2VT/Efni/blob/main/Kennsluefni/ArduinoForritun.md#lesið-inn-frá-serial-monitor)

Munum að alltaf þegar nota á Serial Monitor þarf að setja ```Serial.begin(9600);``` í ```setup``` fallið.

---

### 1.1 Serial Monitor "Hello World!"

Opnaðu Arduino IDE forritið og búðu til nýtt Sketch (File -> New). Það ætti að opnast í nýjum glugga með ```setup``` og ```loop``` föllum.

Skrifaðu svo viðeigandi línu í ```setup``` fallið til að virkja Serial samskiptin.

Skrifaðu svo í ```loop``` fallið viðeigandi línu þannig að þegar forritið keyrir að þá birtist á Serial Monitor "Hello from Arduino".

**Til umhugsunar**, hvernig breytist úttakið í Serial Monitor eftir því hvort þú notar ```print``` eða ```println```.

---

### 1.2 Halló og bless

Aukabjargir: [Skilyrðissetningar](https://github.com/VESM2VT/Efni/blob/main/Kennsluefni/ArduinoForritun.md#skilyrðissetningar)

1. Skrifaðu forrit sem les inn einn staf (```char```) frá Serial Monitor. Ef stafurinn er ```h``` á að skrifa til Serial Monitor **"hallo"** en ef stafurinn er ```b``` á að skrifa **"bless"**.
1. Bættu við forritið: Ef einhver annar stafur er sleginn inn á að birtast á Serial Monitor **"skil ekki!!"**.

---

### 1.3 Í hástafi

Aukabjargir: [Strengir í Arduino (sjá sérstaklega ```toUpperCase()```)](https://www.arduino.cc/reference/en/language/variables/data-types/stringobject/)

1. Skrifaðu forrit sem les inn textastreng frá Serial Monitor og skilar sama streng aftur til Serial Monitor nema að búið er að setja alla stafina í strengnum í hástafi.
1. Gerðu núna forrit með sömu virkni en án þess að nota ```toUpperCase()``` fallið.
   - Vísbendingar:
     - Munurinn á litlum og stórum staf í tölvum er að í hástöfum er fimmti bitinn í stafnum 0 en í lágstöfum er hann 1.
     - Strengur er fylki (svipað og listi í python) af stöfum (```char```).

**Til umhugsunar**, birtist strengurinn aftur og aftur í Serial Monitor? Ef svo er, hvernig getur þú látið hann birtast bara einu sinni. Ef ekki, hvernig getur þú látið hann birtast aftur og aftur.

---

### 1.4 Þín eigin mínustala

Aukabjargir:

- [Strengir í Arduino (sjá sérstakelga ```toInt()```)](https://www.arduino.cc/reference/en/language/variables/data-types/stringobject/)
- Til að snúa bitum er notaður **ekki** (e. not) bitavirkinn (e. bitwise operator) og er táknið fyrir hann ```~``` (tildamerkið).

Skrifaðu forrit sem les inn talnastreng og breytir þeirri tölu svo í mínustölu með því að nota þína eigin útfærslu á [tvíundafyllingu](https://github.com/VESM2VT/Efni/blob/main/Kennsluefni/ArduinoForritun.md#unsinged-hvernig-geyma-tölvur-m%C3%ADnustölur).

---

### 1.5 Fjarstýring

Aukabjargir: [```indexOf()```](https://www.arduino.cc/reference/en/language/variables/data-types/string/functions/indexof/) og [```substring()```](https://www.arduino.cc/reference/en/language/variables/data-types/string/functions/substring/) 

Fjarstýringin fyrir fjarstýrða bílinn sem þú gerir á önninni þarf að senda upplýsingar til bílsins um t.d. hraða og beygjur. Þessar upplýsingar þarf að senda til bílsins sem textastreng (e. string) en verða notaðar af bílnum sem heiltölur.

Til að æfa þig að breyta textastreng í heiltölur ætlar þú að skrifa forrit sem tekur inn textastreng frá Serial Monitor sem inniheldur tvær tölur og kommu á milli þeirra til að aðgreina þær t.d. ```123,456```. Forritið á svo að taka þessar tvær tölur og skila summu þeirra.

---

## Námsmat
- Yfirferð og námsmat á sér stað í tíma. 
- Fyrir hvern lið; Fullt fyrir fullnægjandi lausn/skilning, ekkert ef lausn/skilningur er ábótavant eða vantar. <br>

#### Eftirfarandi er metið í tíma útfrá verklegum tilraunum og skilningi nemanda:

1. Þekkir helstu tög og stærðir í binary. 
1. Getur skrifað út með Serial Monitor (V1.1).
1. Getur lesið frá Serial Monitor (V1.2). 
1. Kann að vinna með skilyrðissetningar og lykkjur í Arduino. 
1. Notar innbyggð föll;`toUpperCase()` og `toInt()`.
1. Notar bitwise operator í lausnum.

<!-- 
1. Þekkir Arduino hardware parta og pinna.
-->

