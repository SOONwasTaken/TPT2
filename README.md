# TPT2
This is where my TPT2 scripts will be housed and updated.

# Current Scripts
Scripts below are most currently updated versions

## T1 Presser Scripts
Because Factory Packages do not currently support T1 Pressers (due to the Hammer recipe being implemented), I've decided to make a few scripts to make them. 

There are 3 scripts, Presser_Main, Presser_Chip, Presser_Hammer. Maximum required lines is 22. The Chip and Hammer scripts are helper scripts with precise values, so there's no **need to edit those**.

### Usage:
- Import package into Facility AI.
- Change the `Impulse` key to whatever you want (Default is `p`).
- Change `Pressers_To_Make` to however many you want.
- Go into the Factory, enable the AI using F4, and press the `Impulse` key.

### Possible Changes / Optimizations:
- ~~Debugging.~~ (Credit: Xenos6666, d0sboots, and Coco)
- ~~Pressers materials are made 1 at a time.~~ (Updated as of v. 2.0)
- Parallel processing.
- Script creates `Pressers_To_Make + 1` pressers due to loop being treated as `while(Pressers_Made <= Pressers_To_Make)`.
- Produces leftovers (Hammer Rods and T1 Cables).
