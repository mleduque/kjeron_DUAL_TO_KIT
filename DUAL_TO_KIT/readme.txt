Dual-class into Kit

Installation Order:
* This mod should NOT be installed BEFORE any mod that adds new kits.
* This mod should NOT be installed BEFORE any mod that alters race(MGSRCREQ.2da/CLSRCREQ.2da) or dualclass(DUALCLAS.2da/ABDCDSRQ.2da) restrictions.
* This mod should NOT be installed BEFORE any mod that alters string references in CLASTEXT.2da, KITLIST.2da, or RACETEXT.2da/SODRACE.2da.
* This mod should NOT be installed BEFORE any mod that alters alignment(ALIGNMNT.2da) restrictions.
* The third component(proficiency) should NOT be installed BEFORE any mod that alters or reads (WEAPPROF.2da).

Limitations(primary component):
* Class/Kit description in the record screen will display the description of the unkitted second class.
* Specialists Mages will not recieve their bonus spell slots. (Fix included in second component.)
* Level-up proficiency selection is still dictated as if an unkitted second class. (Fix included in thrid component.)
(These are all the same issues that occur when you manually change the second-class kit through EEkeeper/Near Infinity)
* Kit-to-Kit dual-classing will replace your current kit with the new one.  Abilities gained through the old kit's CLAB will be retained, but apsects that come from 2da-files or are hardcoded will be lost.

Limitations(proficiency component)
* All (kit or not) dual-classed character's proficiency options will be strictly enforced. Reactivating their original class will not expand their proficiency limitations, they still regain any proficiency that had from that class, they just cannot add to them beyond what their second class normally allows.
* Level requirements for proficiency will continue to follow PROFSMAX.2da.
* Mods that replace a Base class with a kit, should utilize the mods base-class kit proficiency options for the unkitted class, provided the kit and class share the same name. Any character with the base-class kit will use that kits proficiency options as expected.
* Mods that add a Multi-class kit and Single-class kit under the same name will attempt to differientiate them by their kit description. If it fails they might end up using the others proficiency options.
* If it fails to identify class/kit, it should default to FIGHTER or NONE proficiency options, to avoid being stuck during level. This should only happen if their current kit(or trueclass) has been disabled / made invalid by other mods.
* Original WEAPPROF.2da values will be copied to WEAPPROF_backup.2da for reference.

Compatibility:
* v2.3+: BGEE, BGSOD, BG2EE
* v2.5+: IWDEE
* Should work for any language.  Only installation prompts are in English.
* Supports multiple campaign files, as read from CAMPAIGN.2da.
* UI edits have been reworked, should be more compatible with other UI mods.