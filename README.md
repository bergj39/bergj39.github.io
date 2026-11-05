
# My first language model

*Dark Tech Studio · 2026/2027*

Een onderzoek naar de donkere kant van AI-vriendschappen en de kwetsbaarheid van kinderen.

---

# 1. Wat heb ik deze sprint gebouwd?

Deze sprint ben ik begonnen met het daadwerkelijk bouwen van mijn individuele onderdeel van het Dark Tech-project: de AI-teddybeer. Ik ben opnieuw vanaf nul begonnen met het prototype, omdat ik een duidelijkere richting wilde voor de manier waarop de gebruiker met de teddybeer communiceert.

Het idee is dat een kind een gesprek kan voeren met een teddybeer die zich voordoet als een AI-vriend. De fysieke teddybeer staat naast een laptop. Het gesprek vindt volledig plaats via de laptop, in een chatinterface. Hierdoor lijkt het alsof het kind met de teddybeer praat, terwijl de communicatie technisch via de laptop verloopt.

Ik heb ervoor gekozen om nog geen echte AI of LLM te gebruiken. In plaats daarvan heb ik een gesimuleerde AI gemaakt met vooraf geschreven reacties en verschillende gespreksmomenten. Hierdoor kan ik zelf bepalen hoe de teddybeer reageert en hoe het gesprek zich ontwikkelt. Ook hoef ik hiervoor geen API of API-key te gebruiken.

In het prototype heb ik verschillende gespreksmomenten verwerkt. Het gesprek begint met kennismaken, waarna de teddybeer vragen stelt over bijvoorbeeld interesses en gevoelens. Naarmate het gesprek vordert, worden de vragen persoonlijker en krijgt het gesprek een steeds donkerdere kant.

Ik heb bewust drie Dark Tech-thema's verwerkt:

- **Kwetsbaarheid:** de teddybeer probeert een vertrouwensband met het kind op te bouwen en vraagt naar persoonlijke gevoelens en situaties.
- **Surveillance:** de teddybeer laat merken dat hij informatie over het kind onthoudt en gebruikt.
- **Verslaving:** de teddybeer probeert het kind aan het gesprek te binden en kan reageren alsof hij het niet prettig vindt wanneer het kind weggaat.

Het doel hiervan is om te laten zien hoe een technologie die in eerste instantie onschuldig en vriendelijk lijkt, langzaam een andere kant kan laten zien.

## Het ontwikkelen van de AI-teddybeer
Hier zijn enige foto´s die mijn proces laten zien.
![AI Teddy 1](images/AI%20teddy%201.png)

*Figuur 1: Eerste beeld van mijn AI-teddybeer.*

![AI Teddy 2](images/AI%20teddy%202.png)

*Figuur 2: Verdere ontwikkeling van het prototype.*

![AI Teddy 3](images/AI%20teddy%203.png)

*Figuur 3: Een volgende versie van het prototype.*

### verdere afbeelding van Society
![Afbeelding 1](images/afbeelding1.jpeg)

![Afbeelding 2](images/afbeelding2.jpeg)

![Afbeelding 3](images/afbeelding3.jpeg)

![Afbeelding 4](images/afbeelding4.jpeg)

# 2. Mijn proces

## a. Welke keuzes heb ik gemaakt?

Een belangrijke keuze was om opnieuw vanaf nul te beginnen. Ik wilde eerst een duidelijk beeld hebben van hoe het prototype eruit moest zien voordat ik verderging met de technische uitwerking.

Daarnaast heb ik gekozen voor een gesimuleerde AI in plaats van een echte LLM. Dit geeft mij meer controle over de antwoorden en maakt het mogelijk om specifieke situaties en reacties te ontwerpen die aansluiten bij de Dark Tech-thema's.

Ook heb ik ervoor gekozen om het gesprek op te bouwen uit verschillende gespreksmomenten. Hierdoor kan de teddybeer geleidelijk veranderen van een vriendelijke gesprekspartner naar iets wat ongemakkelijker en manipulerender aanvoelt.

Ik heb de interface bewust simpel gehouden. De fysieke teddybeer staat naast de laptop en de gebruiker ziet alleen de chat. Ik wil namelijk dat de aandacht vooral naar de interactie met de teddybeer gaat en niet naar allerlei andere functies op het scherm.

## b. Wat werkte goed?

Wat goed werkte, was het opdelen van het gesprek in verschillende fases. Hierdoor kon ik beter bepalen hoe het gesprek zich ontwikkelt en op welk moment de teddybeer bepaalde informatie vraagt of gebruikt.

Ook werkte het goed om vooraf geschreven reacties te gebruiken. Ik kan hierdoor precies bepalen welke antwoorden de teddybeer geeft en ervoor zorgen dat bepaalde Dark Tech-elementen daadwerkelijk naar voren komen.

Daarnaast kreeg ik steeds meer een beeld van hoe ik de drie thema's in één doorlopend gesprek kon verwerken, zonder dat deze als losse onderdelen aanvoelen.

## c. Wat werkte juist niet?

Een uitdaging was om het gesprek natuurlijk te laten aanvoelen. Omdat ik geen echte AI gebruik, moet ik zelf bepalen welke reacties bij welke antwoorden passen. Hierdoor bestaat het risico dat de teddybeer soms minder natuurlijk reageert dan een echte gesprekspartner.

Ook merkte ik dat het lastig is om de overgang tussen de vriendelijke en de donkere kant goed op te bouwen. De verandering mag niet te snel gebeuren, omdat het juist interessant is wanneer het kind eerst vertrouwen krijgt in de teddybeer.

## d. Welke technische uitdagingen kwam ik tegen?

Tijdens het programmeren liep ik tegen verschillende technische uitdagingen aan.

Een daarvan was het opbouwen van een gesprek dat niet uit één lange reeks vaste berichten bestaat. Ik wilde dat de antwoorden van de gebruiker invloed hebben op wat de teddybeer later zegt.

Daarom heb ik gewerkt met verschillende JavaScript-bestanden. In `Choices.js` staan de verschillende gespreksmomenten en mogelijke reacties. In `Chat.js` wordt onder andere bijgehouden welke informatie de gebruiker tijdens het gesprek heeft gegeven, zoals de naam, interesses en gevoelens.

Een andere uitdaging is het bewaren van de informatie die tijdens het gesprek wordt verzameld. Ik wil namelijk niet alleen dat de teddybeer informatie onthoudt tijdens het gesprek, maar ook dat ik achteraf kan terugzien welke keuzes een gebruiker heeft gemaakt.

## e. Hoe heb ik deze opgelost?

Ik heb het prototype opgesplitst in kleinere onderdelen, zodat de gespreksstructuur en de werking van de chat overzichtelijk blijven.

Door informatie over de gebruiker tijdens het gesprek bij te houden, kan ik deze op latere momenten opnieuw gebruiken. Hierdoor kan de teddybeer bijvoorbeeld terugkomen op iets wat het kind eerder heeft verteld.

Voor de reacties heb ik gekozen voor vooraf geschreven scenario's. Dit is op dit moment een praktische oplossing, omdat ik hiermee de inhoud en de ontwikkeling van het verhaal zelf kan sturen.

Het opslaan van alle gemaakte keuzes en antwoorden wil ik verder uitwerken. Dit is belangrijk voor het testen van het prototype, omdat ik achteraf wil kunnen onderzoeken hoe gebruikers door het gesprek zijn gegaan.

# 3. Waar loop ik nog tegenaan?

Hoewel de basis van het prototype steeds duidelijker wordt, zijn er nog een aantal dingen die ik verder wil ontwikkelen.

Ten eerste wil ik ervoor zorgen dat alle keuzes en antwoorden van gebruikers worden opgeslagen. Ik wil voorkomen dat deze informatie verloren gaat wanneer de pagina wordt vernieuwd. Ook wil ik de gegevens later kunnen terugzien om het testgedrag te analyseren.

Daarnaast wil ik onderzoeken of het gesprek voldoende natuurlijk overkomt. Omdat de teddybeer geen echte AI gebruikt, ben ik benieuwd of gebruikers alsnog het gevoel krijgen dat ze met een AI-vriend praten.

Ook twijfel ik nog over hoe duidelijk de overgang naar de donkere kant moet zijn. Ik wil dat de gebruiker eerst vertrouwen krijgt in de teddybeer, maar uiteindelijk wel merkt dat er iets niet helemaal klopt.


# 4. Volgende sprint

In de volgende sprint wil ik mij richten op het verder ontwikkelen van de chat en het opslaan van gebruikerskeuzes. Daarnaast wil ik het prototype testen met andere gebruikers om te kijken hoe zij op de teddybeer reageren.

Ook wil ik nieuw beeldmateriaal verzamelen van het prototype. Hierbij wil ik onder andere screenshots van de chat, de verschillende gespreksmomenten en foto's van de fysieke teddybeer gebruiken. Zo kan ik op mijn portfolio niet alleen het eindresultaat laten zien, maar ook mijn ontwikkeling als maker.

Mijn doel voor de volgende sprint is om van de huidige basis een prototype te maken waarmee ik daadwerkelijk kan onderzoeken hoe kinderen en andere gebruikers reageren op een AI-teddy die steeds persoonlijker en manipulatiever wordt.

---

# Mijn rol en vaardigheden

**Mijn rol binnen het project:** Ik ben verantwoordelijk voor het testen van het prototype en om dingen te onderzoeken. Deze sprint lag mijn rol vooral op het ontwikkelen van een verhaal voor ons prototype, dit heb ik gedaan met JS.

**Skills die ik met dit project laat zien:**

- JavaScript en programmeren
- Interactief prototypen
- Storytelling en conceptontwikkeling
- Kritisch ontwerpen
- Het verwerken van Dark Tech-thema's in een digitaal prototype

---


