# TaiGu
Almost everything about TaiGu for programmers and font designers.

## Be aware of the facts: (2022.09.13)

1. There are different romanized writing systems of the Taiwanese language.
2. Even within the same romanized writing system, there would be different positioning rules to mark the diacritics, when there is more than one vowel.
3. There are different types of code sequence (in Unicode), sharing among the world wide web.
4. A draft of "Standardization of Taiwanese Writing System" is under preparation.

## About the Programmers:
There are (at least) two types of them:
1. Those who thought, they could control everything.
2. Those who respect to users, even users make mistakes. (So do the programmers.)

## Different Types of code sequence:
1. Nature Writing Order (TW_NWO): the code sequence will be saved as the nature writing order. So, the diacritics will be separated and following the vowels.
2. Unicode NFD (TW_NFD)
3. Unicode NFC (TW_NFC)
4. Unicode NFD with dot less i (TW_NFDi)
5. Mixed (TW_MIX)

## Romanized writing systems:
1. POJ: This system is currently used by the Presbyterian Churchs in Taiwan.
2. POJts: An old system of POJ with the difference: ts will be applied before the vowels a, o, u, instead of ch.
3. TLJ (TL): This system is officially promoted by Taiwan's Ministry of Education.

## Positioning rules:
1. ttv: The rule used in <<The Holy Bible, Today's Taiwanese Version, Romanized Edition>> for POJ.
2. To be added.

### The difference between TW_NWO and TW_NFD
The Taiwanese vowel o͘ with a tone mark (diacritic) has different code seqence in TW_NWO and TW_NFD.

The vowel o͘ is a composition of o + U+0358, since the tone mark will be given after the vowel in speaking. So the nature wrinting order follows this speaking sequence.

* That code sequence in TW_NWO is: o, U+0358, U+030X. Where U+030X are diacritics.

* That code sequence in TW_NFD is: o, U+030X, U+0358. Where U+030X are diacritics. This order comes from the normalization algorithm of Unicode.
