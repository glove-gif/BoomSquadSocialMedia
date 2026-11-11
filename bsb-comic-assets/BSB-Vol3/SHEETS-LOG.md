# BSB Super Comic Vol. 3 "Mega Punch Bunch!" — character/prop sheets log
Started 2026-11-11. Method: ChatGPT in Chrome, new chat per sheet, 3 refs attached (robot TBS sheet, Mom BSB sheet = style/layout, twin's BSB hero sheet = proportions). Send via .ProseMirror insertText + button whose aria-label contains "Send". Download via JS blob of img[alt^="Generated image"] -> stage ~/mnt/Downloads. Push: vol3/vpipe.sh (bpipe.sh pointed at bsb-comic-assets/BSB-Vol3/).
Twin hero sheets: cover/refs/BSB-{Baboom,Buster,BlastCaptain}-Hero-Sheet-NoHands.jpg; /mnt/user-data/uploads/assets/BSB/_references/BSB-{Scout,Gavel,Ratchet}-Hero-Sheet-NoHands.png

## Base prompt (worked)
(see bottom of file)

## Sheets
- Robo-Baboom: sheets/BSB-Robo-Baboom-Sheet.png — 1st try accepted; hands zoom-checked OK (guide 3+thumb; figure hands are fists). Note: ChatGPT added a small yellow V belly emblem (BSB suit template).
- Robo-Buster: sheets/BSB-Robo-Buster-Sheet.png — hands OK 1st try; fix 1 (edit-only): green decorative strokes/bottom bar -> light blue. v1 kept as -v1.png.
- Robo-Scout: sheets/BSB-Robo-Scout-Sheet.png — hands OK 1st try; fix 1 (edit-only): added missing THUMBS UP label. v1 kept.
- Robo-Gavel: sheets/BSB-Robo-Gavel-Sheet.png — fix 1 (edit-only): thumbs-up redrawn to clearly show 3 curled fingers + thumb. Afro (no swoop) per his robot sheet. v1 kept.
- Robo-Ratchet: sheets/BSB-Robo-Ratchet-Sheet.png — 1st try accepted; hands zoom-checked OK. Weapon panel = Robo-Hoverboard (main/side/bottom).
- Robo-Blast Captain: sheets/BSB-Robo-BlastCaptain-Sheet.png — 1st try accepted; hands OK. No weapon on his TBS sheet, so bottom-left panel = MECHANICAL DETAILS (head/backpack/chest). Twin ref = BSB-BlastCaptain-Hero sheet; build reads big chest/small waist/Popeye forearms.

- Heal-O-Matic 5000: sheets/BSB-Heal-O-Matic-5000-Prop-Sheet.png — 1st try accepted (front, side, active glowing, palette, features + control panel). Minor: in side view the gold chevron reads as a small fin.

ALL 7 SHEETS DONE 2026-11-11; pushed to GitHub bsb-comic-assets/BSB-Vol3/. Awaiting Aaron review.

## Prompts that worked (robot template; {placeholders} filled per robot; also in Chrome localStorage.v3tpl)
Image 1 = {NAME}'s TBS character sheet. Image 2 = Mom's approved BOOM SQUAD BUDDIES (BSB) sheet: copy its STYLE and LAYOUT exactly. Image 3 = BSB {TWIN} hero sheet: copy its BODY PROPORTIONS exactly.
Redraw this robot as a BOOM SQUAD BUDDIES character sheet in exactly the style of the BSB sheet. Keep every design detail, color and accent glow from the robot's sheet.
STYLE: very round big head (about 2/5 of total height incl. hair), thin noodle limbs, big cartoon hands, HUGE chunky boots each about as wide as the torso. Bold thick black outline plus one white sticker stroke around each figure. Flat 2-tone color (base + one shadow), no gradients, no texture, no shine streaks (the accent glow may be a flat lighter color).
HANDS: EXACTLY 3 fingers + 1 thumb on EVERY hand, always. Robot hands but still 3 fingers + 1 thumb.
HAIR: same shape and color as on the robot's sheet, simplified into a few big chunky spikes, the tall swoop rising on the NOSE side in side view. Visor goes right up to the hairline. NO STRAP on the visor (no band past the temples or behind the head).
The character never wears his weapon on his body (not on the back or hip); the weapon appears ONLY in the weapon panel.
{EXTRA: per-robot colors/details + "Accent color for the decorative strokes and bottom bar: <color>."}
LAYOUT (landscape, like image 2): "BOOM SQUAD BUDDIES" logo header top-left exactly like image 2, big name "{UNAME}" with tagline "{TAG}", top row FRONT (RELAXED), SIDE VIEW, BACK VIEW, TOP VIEW; COLOR PALETTE column on the right; bottom-left panel "{WEAPON}" with main / side / angled views; bottom-right panel "HAND GUIDE" with the line "ALWAYS 3 FINGERS + 1 THUMB" and robot hands: open hand, fist, pointing, thumbs up. Bottom bar with the chevron like image 2. NO "Signature Pose" panel. White background. Spell every label correctly.

Per-robot EXTRA used:
- Baboom: black/dark-gray armor, glowing GREEN accents/visor, green hexagon core, black spiky hair. Weapon THE ROBO-BOOMERANG.
- Buster: metallic-gray chest plate, LIGHT-BLUE accents/visor/hex core, black pompadour; THE ROBO-BOOMSTICK (hits, no electricity). Accent strokes light blue (added via fix).
- Scout: girl robot, RED accents/visor, red triangle core, high collar + armored coat tails, long wavy black hair; THE ROBO-SAFESTRIKE SHIELD (pentagon, red double chevron). Template pronouns his->her.
- Gavel: a little taller, big metallic-gray shoulder armor, YELLOW accents/visor/hex core, round afro (HAIR line replaced: "same round afro ... chunky puffs", no swoop); THE ROBO-MEGASLAM HAMMER.
- Ratchet: ORANGE accents/visor/pentagon core, high collar + long coat with orange edges, headphone discs; THE ROBO-HOVERBOARD (main/side/bottom views).
- Blast Captain: BSB Blast Captain build (bigger, barrel chest, small waist, Popeye forearms), clean GLOSSY purple armor, gray backpack thrusters, visor down, black hair magenta tips, magenta accents; weapon line removed; bottom-left = MECHANICAL DETAILS (HEAD/BACKPACK/CHEST DETAIL). Tagline VYLEX'S ULTIMATE CREATION.

Edit-only fix prompts (one fix per message, same chat):
- "EDIT-ONLY. Keep this whole sheet exactly the same (every character, hand, label, layout, size). Change ONLY the green decorative strokes to glowing light blue (#22B8FF) ..." (Buster)
- "EDIT-ONLY. ... Add ONLY the missing label "THUMBS UP" (two lines) under the thumbs-up hand ... same hand-lettered font" (Scout)
- "EDIT-ONLY. ... Change ONLY the THUMBS UP hand ...: clearly 1 raised thumb plus EXACTLY 3 curled fingers, each a separate rounded segment with bold black outline ..." (Gavel)

Heal-O-Matic 5000 prompt: Chrome localStorage.v3heal (refs: Mom BSB sheet + BSB Robo-Buster sheet for style/layout).
