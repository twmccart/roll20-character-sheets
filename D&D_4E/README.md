Useful Attributes:

level // current level.
halflevel // current half level.

hp // current and max hit points.
hp-bloodied // bloodied value.
surge-value // your surge value.
surges // current and max number of surges daily.
tmp-hp // temporary hit points.

initiative // your initiative mod, this + 1d20 = your initiative. (Todo: Add roll button if Riley adds buttons with text.) 

speed // your speed in squares.

action-points // your current number of action points.

ac // your amour class.
fort // your fortitude.
ref // your reflex.
will // your will.

// attribute scores:
strength
constitution
dexterity
intelligence
wisdom
charisma
*attribute from above*-mod // (ie strength-mod) attribute modifier.
*attribute from above*-mod-level // (ie strength-mod-level) attribute modifier with half level.

passive-insight // your passive insight.
passive-perception // your passive perception.

// skills (all with half level). (Todo: Add roll button if Riley adds buttons with text.) 
acrobatics
arcana
athletics
bluff
diplomacy
dungeoneering
endurance
heal
history
insight
intimidate
nature
perception
religion
stealth
streetwise
thievery

Powers:

Powers are a repeating section, so they can be dragged into any order, added and
deleted like the rest of the sheet, and are no longer capped at 100.

Characters made before this change are migrated automatically the first time the
sheet is opened: each filled power slot becomes a row. The old power-[number]-*
attributes are left in place and are simply no longer shown, so nothing is lost,
but note that they stop tracking the power - a macro elsewhere that refers to
@{power-3-macro} will keep returning the value it had at migration time.

To reference a power from a token action or macro, use its position in the list
rather than a fixed number:

%{CharacterName|repeating_powers_$0_power} // the first power
%{CharacterName|repeating_powers_$1_power} // the second, and so on

Each power picks where its attack, damage, dice count and dice size come from:
one of the six weapons, or a flat value set on the power itself. The Weapon
dropdown sets all four at once; choosing Custom exposes them individually, so a
power can still draw its attack from one weapon and its damage from another.

Updates:

2014-04-23 14:27 :
Added Attack workspace and started item management.

2014-04-16 19:26 :
Full CSS reworking, almost all styles now controlled by css file (not dependant on roll20's base css file).

-Alex L.

2014-04-12 21:25 :
As everything in the D&D 4E sheet is now pretty much in working order, a proper readme file detailing special use cases and general how-to's could be useful? Intent would be for someone with zero knowledge of code should be familiar with how to use the sheet after reading this file. -Ville S.

2014-04-09 20:23 :
Updated html and css to resemble classic B/W 4th Edition character sheet.

ToDo:
Rolls - Waiting on Rileys response re:Buttons with text.

-Alex L.
