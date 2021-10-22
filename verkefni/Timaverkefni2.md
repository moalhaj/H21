# Tímaverkefni 2

- Einstaklingsverkefni.
- Settu upp verklega með brauðbretti og íhlutum.

---

#### 2.1 - DHT11 og serial monitor (20%)

Skoðaðu [þessa grein](https://lastminuteengineers.com/dht11-module-arduino-tutorial/) um hita og rakaskynjarann DHT11 og settu upp fyrri rásina í greininni (það á ekki að setja upp rásina með LCD skjánum).

1. Bættu tveimur LED perum við rásina. Önnur peran á að lýsa ef að hitastigið fer upp fyrir 35°C en hin á að lýsa ef rakastigið fer niður fyrir 50%. 
   
<!-- #### Til að auka rakastigið þá andað á DHT11.-->
<!-- #### Til að auka hitastigið þá nota hitagjafa; kveikjara.-->
<!-- #### KANNSKI Tilt sensor. -->

---

#### 2.2 - 7-Segment ein tala (20%)

Kynntu þér hvernig 7-Segment virkar með því að lesa [þessa grein](https://lastminuteengineers.com/seven-segment-arduino-tutorial/).

Til umhugsunar:

- Hvort er þitt 7-Segment Display *common anode* eða *common cathode*?
- Hver er munurinn á þessu tvennu?

Í greininni er sýnd útfærsla á teljara. Settu teljarann upp á brauðbretti og settu kóðann á Arduino tölvuna þína **en farðu eftir [þessari mynd](https://raw.githubusercontent.com/VESM2VT/Efni/main/Myndir/SevenSeg_1_vidnam.png) til að tengja 7-Segment-ið**, notar bara eitt 1KΩ viðnám í stað átta 220Ω viðnáma.

1. Þú veist að ```loop``` fallið er lykkja en í kóðadæminu er eina sem er í fallinu ```for``` lykkja. Breyttu útfærslunni á fallinu þannig að það þurfi ekki að nota "auka" lykkju.
1. delay() veldur oft truflunum á 7-segment. Breyttu kóðanum þannig að þú notar `millis()`

---

#### 2.3 - Teningur (20%)
1. Útfærðu teninginn (Rolling Dice) sem er neðst í [greininni](https://lastminuteengineers.com/seven-segment-arduino-tutorial/) en breyttu útfærslunni þannig að þú þurfir ekki "pullup" viðnámið heldur sé það leyst í kóða. Bættu líka við "debounce" á takkann.

---

#### 2.4 - 7-Segment fjórar tölur (20%)

Kynntu þér hvernig 7-Segment með fjórum tölustöfum virkar með því að lesa seinni hluta [þessarar greinar](https://www.circuitbasics.com/arduino-7-segment-display-tutorial/) (kaflinn *4 DIGIT 7-SEGMENT DISPLAYS*). Skoðaðu einnig stillingar og aðgerðir í [SevSeg safninu](https://github.com/DeanIsMe/SevSeg). Settu upp fyrri rásina (sem birtir 4.999). Það á ekki á að setja upp seinni rásina (DISPLAYING SENSOR DATA).

1. Skrifaðu forrit fyrir niðurteljara sem vikar með 4 stafa 7-Segment-inu. Forritið á að lesa inn heiltölu frá Serial Monitor og telja svo frá þeirri tölu niður í núll. Þegar komið er í núll á teljarinn að byrja aftur að telja frá því gildi sem hann var stilltur á upphaflega. Hafðu líka takka sem endurstillir talninguna í upphafstöluna þegar ýtt er á hann.

---

#### 2.5 - 7-Segment 4 tölustafir með dht11 og takka. (20%)

1. Settu upp rás sem getur mælt hita og rakastig og birt það á 4 tölustafa 7-Segment skjá. Það þarf að vera hægt að skipta á milli þess hvort skjárinn sýnir hita eða raka stig með takka.

Dæmi um útfærslu:

![Hitastig - Rakastig](https://raw.githubusercontent.com/VESM2VT/Efni/main/Myndir/v1_v21.gif)

---

## Námsmat og skil
Yfirferð og námsmat á sér stað í tíma. <br>
Fyrir hvern lið; gefið er heilt fyrir fullnægjandi lausn, hálft ef lausn er ábótavant, ekkert ef lausn er stórlega ábótavant eða vantar. 

Skilaðu á Innu vefslóð á **Github repo** (private) með `.md` skrá sem inniheldur:

1. myndbönd af virkni úr verklegum tilraunum.
   - Passaðu að nafnið þitt og dagsetning komi fram (t.d. á miða) í öllum myndböndum.
1. kóðalausnir.


<!--
#### Takki + pullup/down viðnám (%) 
- tutorial óbreyttur, tímaverkefni

1. tímaverkefni; birta tölu, teljari, teningakast.
1. Hvort er þitt 7-Segment Display *common anode* eða *common cathode* og hver er munurinn á þessu tvennu?
1. 7-Segment Display samanstendur af 8 LED, hvers vegna þarf bara eitt viðnám (en ekki átta)?
1. Útfærðu teljara (Count Up Timer) með 7 segment display þannig að hann noti ekki `for` lykkjuna.

-->
