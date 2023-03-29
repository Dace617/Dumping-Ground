
# Bug Breakdown

Going through most of the bugs on clickup, I will rank them by (my own thoughts on) severity. Starting with bugs that are causing game crashes and/or quests to be uncompletable, etc. then moving on to smaller but still important-ish issues like missing textures, misplaced NPCs etc.

---

## General To-Do.


A general overview of the large issues that may/may not be related to several bugs, just a nice bullet point for you to look at first.

- Fix up load order using Hajo and I's fixed loadorder.txt on reminders [Clickup](https://app.clickup.com/t/860q90b69)
- Add my fix for the bodies of various NPCs being naked when unclothed, linked in the [Uthgerd Bug Report](https://app.clickup.com/t/863g428f9)
- Unsure if we want to think about other changes to the main profile, it seems to be hitting people pretty hard even with good systems with stuttering etc. might be worth dropping some of the textures/looking at the LODs again or something so we can smooth that out a bit for the regular profile.
- Add in all the fixed bugs in the Fixed column (duh)
- most notably is the Economy Overhaul perk fix by Hajo, if you only add one thing from the fixed column it should probably be this, other than the load order fixes.
- Update Slow your Roll ini with fixed Misc objectives line linked [here](https://app.clickup.com/t/860qcfjr2)
- add the various patches from the Patches reminders section. they fix quite a few bugs/issues.
- Hajo has a race patch fix in the Fixed bug section that should fix a lot of issues.
- Poison Spray CTDs, Helgen Reborn CTDs(This one is likely Load order related), and Winking Skeever CTDs are the major crashes we have reported/know about that I can remember.
- There's a reasonably large issue with 
- I've listed out the largest bugs here with fine details, short of Animation issues (which we didn't get a lot of info about) thses seem to be the largest issues.
- The rest of the bugs not mnentioned are things like various floating NPCs, bad textures etc. that we can fix individually with patches, if you want finer details I can edit this and add them, I'll just sit down and patch what I can after I get this to you.

## Severe Bugs


### Has Fix
---

Bug: Load order in performance Profile is massively broken

Clickup Link: https://app.clickup.com/t/860q90b69

Severity: High, could fix a myriad of other issues

Fix: Load loadorder.txt from clickup reminder into LS4 - Performance Profile.

Other Info: After installing check both load orders to make sure EnhancedAIFramework.esm is loaded before OrganicFactions.esm in both profiles

---


## No Fix (Fix Unknown)

Bug: Equipment Toggle causing crashes with certain hair styles.

Clickup Link: https://app.clickup.com/t/8669m2zer

Severity: High, causing crashes

Fix: Unkown, but I believe MS had a similar issue that we fixed, unsure how.

Other Info: exact hair that was causing the crash listed in bug report.

---

Bug: Winking Skeever Loft crash

Clickup Link: https://app.clickup.com/t/8669ku6ch

Severity: High but inconsistent

Fix: Unkown, possible mesh/lux related?

Other Info: As noted on the comment, I could replicate a crash after buying the loft, but it was not identical to the user that reported it, it was crashing on an 
entirely different mesh.

---

Bug: CTD with poison spells

Clickup Link: https://app.clickup.com/t/860q0rw29

Severity: High

Fix: Unkown, yet to test this one. Seems widespread through nearly every posion effect, as we've had reports of nearly every type of spell, possibly Mysticism/patch 
related?

Other Info: N/A haven't got to testing this one yet.

---

Bug: Misc Quests giving Experience

Clickup Link: https://app.clickup.com/t/860qcfjr2

Severity: Medium

Fix: Replace Slow your Roll ini with one linked on clickup.

Other Info: This fixes a lot of the "quest is repeatable infintie exp" bug reports.

---

Bug: Various users hitting Reference Limit

Clickup Link: N/A

Severity: High-ish?

Fix: No Idea

Other info: We've had about half a dozen reports of this, we've fixed a couple of issues of it, with the critter spawning etc. but there are still people getting the 
error, figured I'd mention it as it's only come up in discord chats, Graven and I have been looking into it, but haven't found a cause or any real commonality between the occurances. It's increasingly hard to get decent info out of the users that have this issue and I can't replicate it myself.

---

Bug: Wait animation apparently causes the FOV lock bug

Click Up Link: https://app.clickup.com/t/862je03je

Severity: Medium-High

Fix: Disabling the wait animation (so it stops forcing camera switch should work

Other Info: Have had additional reports (just in discord) that the poison weapon animation just does a weird idle pose instead of animating any actual posion on the weapon, so it might be worth just yeeting this mod entirely given the issues we've had with it? seems a bit superfluous if we just have to disable everything in it to stop it causing issues.

