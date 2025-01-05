# FightClub5e
Fight Club 5e updates

All credit to [ViannaEuphoria](https://www.reddit.com/user/ViannaEuphoria/) and the [Archivist](https://www.reddit.com/user/FightClub_Archivist/) for their incredible work. They did the bulk of the work. I'm just adding a few modifications.

Steps to replace 2014 data with 2024 data:
1. Download and edit [WotC_2024+UnearthedArcana](https://github.com/vidalvanbergen/FightClub5eXML/releases/download/2024.12.31/WotC_2024+UnearthedArcana.xml) Compendium
2. Replace " [2024]" with "".
3. Replace "Paladin (Ancient)" with "Paladin (Ancients)".
4. Replace " Of " with " of ".
5. Replace " of The " with " of the ".
6. Replace "Artificer (UA)</classes>" with "Artificer, Artificer (UA)</classes>".
7. Replace "Artificer (UA) (Alchemist)</classes>" with "Artificer (Alchemist), Artificer (UA) (Alchemist)</classes>".
8. Replace "Artificer (UA) (Armorer)</classes>" with "Artificer (Armorer), Artificer (UA) (Armorer)</classes>".
9. Replace "Artificer (UA) (Artillerist)</classes>" with "Artificer (Artillerist), Artificer (UA) (Artillerist)</classes>".
10. Replace "Artificer (UA) (Battle Smith)</classes>" with "Artificer (Battle Smith), Artificer (UA) (Battle Smith)</classes>".

If you want to keep both the 2014 & 2024 versions of any of these categories, then do the following:
1. If you want to keep the 2014 & 2024 versions of Races, then search for <race> and for each race
   Replace "</name>
    <size>" with " [2024]</name>
    <size>"
2. If you want to keep the 2014 & 2024 versions of Backgrounds, then
   Replace "</name>
    <proficiency>" with " [2024]</name>
    <proficiency>"
3. If you want to keep the 2014 & 2024 versions of Classes, then
   Replace "</name>
    <hd>" with " [2024]</name>
    <hd>"
4. If you want to keep both the 2014 & 2024 versions of Spells, then
   Search for "<name>Acid Splash" and after that,
   Replace "</name>
    <level>" with " [2024]</name>
    <level>"

A few spells in 2014 got renamed in 2024, so we need to rename them in the 2014 Repository:
1. Download and edit [WotC_2014+PartneredContent+MercerBrew](https://github.com/vidalvanbergen/FightClub5eXML/releases/download/2024.12.31/WotC_2014+PartneredContent+MercerBrew.xml) Compendium
2. Search for "Feeblemind" (not case sensitive) and Replace with "Befuddlement".
3. Search for "Summon Draconic Spirit" (not case sensitive) and Replace with "Befuddlement".
4. Search for "Branding Smite" (not case sensitive) and Replace with "Shining Smite".

Order to load these edited Collections:
1. Load the edited WotC_2014+PartneredContent+MercerBrew collection
2. Load the edited WotC_2024+UnearthedArcana collection

Attached Collections have been adjusted as above (keeping both versions of Races, Backgrounds, Classes, and Spells).
* The 2024 Classes were pulled out and worked out in a separate document, since there were a large number of changes I made to better integrate them (none of them involving changing anything from official release data).

Upcoming Work to be completed:
* Adding Familiar versions of all possible Familiars for the Find Familiar options, edited to make all Familiars more viable options (rather than the default owl)
* Appending " [2014]" after 2014 race/background/class/spell names (only the ones converted to 2024), to allow combining the 2014 and 2024 untagged data together
  * This should ensure that references to this data from Monsters/Classes/Items etc point to the updated 2024 updated version if available, while keeping the 2014 version of historical reference
