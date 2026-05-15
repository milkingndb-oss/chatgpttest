# Project Handoff Guide

This file is the complete handoff note for migrating the project to another account or chat. A new AI assistant should read this first, then inspect the project files named below before making changes.

## Project Folder

Current project path:

`C:\Users\WarLock\Desktop\1sspuppyproject\codex`

The project is a narration-based fantasy/action progression story built from an original PDF transcript and a large set of character profile images. The current deliverables are:

- A completed rewritten story for about a 64-minute narration video.
- An atomic scene breakdown JSON for image generation.
- A location bible for visual consistency.
- Character/profile image PNGs for all story characters and monster forms.
- A `scene_images` folder containing generated images through the cleaned first-five-minute hook.

## Essential Files

These are the core files that must be preserved:

- `puppy-transcript.pdf`
  - Original source transcript.
  - Extracted earlier as about **95 PDF pages**, **229,927 characters**, and **39,331 words**.
  - The transcript ends mid-Wooan arc, so the rewritten story follows it broadly until that cutoff, then completes the plot with an original continuation using the same project roster and factions.

- `completed-rewritten-narration-story.md`
  - Final rewritten story.
  - Current count after the stronger hook addition: **10,143 words**, **58,643 characters**, **858 lines**.
  - Target runtime: about **64 minutes** at normal narration speed.
  - Starts with a future-scale cold open to hook viewers, then rewinds to Chenlin's original summoning humiliation.

- `scenebreakdown.json`
  - Atomic image-generation scene plan.
  - Current count after duplicate-scene cleanup: **204 total scenes**.
  - **59 first-five-minute hook scenes**: `F5_001` to `F5_060`, with duplicate `F5_046` removed.
  - **89 first-ten-minute dense opening scenes**: cleaned `F5` hook block plus `T10_091-T10_120`.
  - Duplicate meat-buying, first-feeding, and contractor-feedback beats after scene 30 were removed.
  - Every scene includes: `id`, `title`, `storyMoment`, `location`, `cameraViewType`, `requiredCharacters`, `statCardRequired`, `statCardReason`, and `imagePromptNotes`.
  - All **82 PNG character/profile variants** are referenced at least once.

- `location-bible.md`
  - Visual consistency bible for locations and global art direction.
  - Defines all locations used by the scene breakdown, including `Wooan Base Command Center`, which was added after audit.

- `scene_images\`
  - Output folder for generated scene images.
  - Already contains:
    - `scene_001_F5_001.png` through `scene_059_F5_060.png`

## Current Story Summary

The story follows **Chenlin**, a poor summoner from an ordinary family. At his awakening ceremony, everyone expects him to summon a powerful beast, but he summons a tiny black puppy. His classmates laugh, his teacher **Luen** is disappointed, and his girlfriend **Lu Ru Yan** leaves him for the stronger spear knight **Luang**.

Chenlin secretly recognizes that the puppy has a hidden devouring bloodline. He accepts a painful lifebound contract and names the puppy **Hey Ming**. The hidden talent **Gluttonous Greed** lets Hey Ming convert consumed matter into growth energy and feed part of that power back into Chenlin.

The story then progresses through:

1. Chenlin's family sacrifice and the last coin from his little sister.
2. Public humiliation at the awakening ceremony.
3. Lifebound contract and Gluttonous Greed reveal.
4. Hey Ming's first feeding and first evolution.
5. Entrance exam in Burial Bone Forest.
6. Goblin swarm, goblin cave, and Troll Boss fight.
7. Scoreboard shock and academy recruitment.
8. Chenlin choosing **Yunk Academy**.
9. Introduction of academy classmates and humanity's hidden war crisis.
10. Summoning **Silver Butterfly**, which becomes living armor/weaponry through rare metal fusion.
11. Disaster Trial and defeat of the **Disaster Matriarch**.
12. Summoning **Diana**, a young angel rescued from a corrupted sacred realm.
13. High-level mountain missions: Berserk Black Ape, Twin Fang Giant Tiger, Giant Rock Drake, Blood Spirit Colossal Crocodile.
14. Fallen Clan and Shadow Congregation border ambush.
15. Balian Mountain purge against multiple colossal beasts.
16. Wooan Base defense and the massive beast tide.
17. Diana's moon/ring-blade form.
18. Dark Gold Berserk Bear King boss battle.
19. Final Fallen Clan gate invasion.
20. Fallen Sky Phantom breach and academy support line.
21. Diana's Sun-Moon Judgment.
22. Hey Ming devouring the invasion gate.
23. Diana's sacred realm restoration.
24. Yunk Academy epilogue with Hey Ming statue.
25. New spatial disturbance and next-horizon ending.

## Important Creative Constraint

The rewritten story is not a word-for-word translation of the transcript. It is a cleaned, rephrased, completed narration story that uses the same core premise, characters, powers, factions, and progression-fantasy structure. Because the original PDF stops mid-arc, the ending is an original continuation designed to fit the established project.

Do not claim the ending is the original transcript ending.

## First Five Minutes Hook Strategy

The story now begins with a cold open:

- Hey Ming as a world-scale black-flame wolf over Wooan.
- Diana splitting the sky with a crimson moon.
- Silver Butterfly armor and the Fallen Clan warlord.
- Hey Ming devouring an invasion gate.
- Then the narration rewinds to the poor rented room and the mocked puppy summon.

In `scenebreakdown.json`, the first five-minute hook block is:

- `F5_001` to `F5_060`
- duplicate `F5_046` removed from the actual scene array
- cadence: one image beat every **4-6 seconds**
- strategy: future payoff, betrayal, humiliation, hidden power, and first feeding cliffhanger

The first ten minutes are:

- cleaned `F5_001-F5_060` hook block, minus duplicate `F5_046`
- `T10_091-T10_120`
- cadence: **4-6 seconds**
- coverage: cold open through Hey Ming's growth, then quiet bond, first evolution, and exam transition

Later scenes can use a slower cadence:

- about **25-35 seconds** per image
- faster during battles, transformations, and stat-card moments

## Character Name Normalization

The original transcript had many misspellings and machine-translation variants. Use these normalized names:

- `Chenlin`, `Chen Lin`, `Chenllin` -> **Chenlin**
- `Hey Ming`, `Hay Ming`, `Haying`, `Haing`, `Heiming` -> **Hey Ming**
- `Lu Ruan`, `Lu Ruen`, `Lu Ru Yan` -> **Lu Ru Yan**
- `Su Ling Shu`, `Suling Shu`, `Suling Shuer` -> **Su Ling Shu**
- `Cao Wu`, `Caoou`, `Caoyu`, `Sao Wu` -> **Commander Cao Wu**
- `Yang Sha`, `Yang Shia`, `Yong Xiao`, `Yang Xiao` -> **Yang Xiao**
- `Wooan`, `Wuan`, `Wooan City` -> **Wooan**

## Character/Profile Image Roster

All of these PNG files are in the project root and should be treated as character/profile references for image generation:

### Chenlin And Family

- `Chenlin_CL-F0.png`
- `Chenlin_CL-F1.png`
- `Chenlin_CL-F2.png`
- `Chenlin_CL-F3.png`
- `Chenlin_CL-F4.png`
- `Chenlin_Little_Sister.png`
- `Chenlin_Mother.png`

### Hey Ming Forms

- `Hey_Ming_HM-F0.png`
- `Hey_Ming_HM-F1.png`
- `Hey_Ming_HM-F2.png`
- `Hey_Ming_HM-F3.png`
- `Hey_Ming_HM-F4.png`
- `Hey_Ming_HM-F5.png`
- `Hey_Ming_HM-F6.png`
- `Hey_Ming_HM-F7.png`

### Diana Forms

- `Diana_DI-F0.png`
- `Diana_DI-F1.png`
- `Diana_DI-F2.png`
- `Diana_DI-F3.png`
- `Diana_DI-F4.png`

### Silver Butterfly Forms

- `Silver_Butterfly_SB-F0.png`
- `Silver_Butterfly_SB-F1.png`
- `Silver_Butterfly_SB-F2.png`
- `Silver_Butterfly_SB-F3.png`
- `Silver_Butterfly_SB-F4.png`

### Academy, Allies, And Human Characters

- `Commander_Cao_Wu.png`
- `Fang_Ya.png`
- `Fang_Yi.png`
- `Ji_Fei.png`
- `Ji_Kong.png`
- `Jiang_Ju.png`
- `Jiang_Wu.png`
- `Joe_Yuan.png`
- `Li_Mingji.png`
- `Lia_Curly_LC-F1.png`
- `Lia_Curly_LC-F2.png`
- `Lu_Hongying.png`
- `Lu_Ning.png`
- `Lu_Ru_Yan.png`
- `Lu_Xiaoyu.png`
- `Luang.png`
- `Luen.png`
- `Luolan.png`
- `Luolu.png`
- `Luwan.png`
- `Meow_Shan_Shan.png`
- `Su_Ling_Shu.png`
- `Wang_Yao.png`
- `Wangfeng.png`
- `Xiao_Huiyang.png`
- `Xiao_Yang.png`
- `Xiao_Yun_Shu.png`
- `Ya_Chowo.png`
- `Yang_Xiao.png`
- `Yi_Kexi.png`

### Fallen Clan, Cultists, Enemies, And Monsters

- `Berserk_Black_Ape.png`
- `Blood_Spirit_Colossal_Crocodile.png`
- `Dark_Gold_Berserk_Bear.png`
- `Delicate_Assassin_Woman.png`
- `Disaster_Matriarch_DM-F1.png`
- `Disaster_Matriarch_DM-F2.png`
- `Fallen_Clan_FC-F1.png`
- `Fallen_Clan_FC-F2.png`
- `Fallen_Clan_FC-F3.png`
- `Fallen_Clan_FC-F4.png`
- `Fallen_Sky_Phantom_FS-F1.png`
- `Fallen_Sky_Phantom_FS-F2.png`
- `Giant_Rock_Drake.png`
- `Golden_Haired_Lightning_Caster.png`
- `Hulking_Flame_Man.png`
- `Leakru_LK-F1.png`
- `Leakru_LK-F2.png`
- `Leardis_LD-F1.png`
- `Leardis_LD-F2.png`
- `Raging_Horned_Bull.png`
- `Shadow_Congregation_Cultists_SC-F1.png`
- `Shadow_Congregation_Cultists_SC-F2.png`
- `Three_Headed_Serpent.png`
- `Troll_Boss.png`
- `Twin_Fang_Giant_Tiger.png`
- `Twisted_Tree_King.png`
- `Undying_Berserk_Bear.png`

## Generated Images So Far

Generated scene images are stored in:

`scene_images\`

Completed:

- `scene_images\scene_001_F5_001.png` through `scene_images\scene_059_F5_060.png`
  - Current generated count: **59 sequential scene images**
  - Current frontier:
    - `scene_images\scene_059_F5_060.png`
    - Scene ID: `F5_060`
    - Title: `First Five Minute Cliffhanger`
  - Sequence audit:
    - filenames are sequential with no gaps from `scene_001_*` to `scene_059_*`
    - each filename includes the matching `scenebreakdown.json` scene ID

Next image to generate:

- `scene_images\scene_060_T10_091.png`
  - Scene ID: `T10_091`
  - Title: `Quiet Bond: Chenlin sits beside Hey Ming`

## Image Generation Workflow

When generating scene images:

1. Read `scenebreakdown.json`.
2. Select the next scene by order in `scenes`.
3. Load/view each `requiredCharacters[].profileImage` as reference before generating.
4. Build a prompt using:
   - scene `title`
   - `storyMoment`
   - `location`
   - `cameraViewType`
   - `requiredCharacters`
   - `statCardRequired`
   - `statCardReason`
   - `imagePromptNotes`
   - visual rules from `location-bible.md`
5. Generate a 16:9 cinematic image unless the user asks otherwise.
6. Save the generated file into:
   - `scene_images\scene_###_<sceneID>.png`
7. Keep numbering aligned with scene order and include the scene ID:
   - first scene -> `scene_001_F5_001.png`
   - second scene -> `scene_002_F5_002.png`
   - sixtieth scene -> `scene_060_T10_091.png`
8. Leave the original generated image in Codex's default generated-images folder; copy it into `scene_images`.
9. Do not overwrite existing scene images unless explicitly asked. If regenerating, use a versioned name such as `scene_060_T10_091_v2.png` or ask first.

### Prompt Style For Scene Images

Use this structure:

```text
Use case: illustration-story
Asset type: 16:9 cinematic scene image for scene <ID>, save-worthy production still
Primary request: <scene title and story moment>
Input images used as character reference: <list profile filenames and what to preserve>
Scene/backdrop: <location from scene + location bible notes>
Subject: <main visual action>
Style/medium: high-end anime fantasy key visual, cinematic painterly concept art
Composition/framing: <cameraViewType>
Lighting/mood: <mood from story and location bible>
Color palette: <consistent palette>
Constraints: preserve character design from profile references; no text, no labels, no watermark, no UI overlays unless the scene explicitly requires a stat/system card
```

For stat-card scenes:

- If the image itself should show the card, include a clean translucent blue-black fantasy system UI.
- Keep any text short and legible.
- If exact text is not necessary, use abstract stat-card shapes rather than readable text to avoid text errors.

## Visual Consistency Rules

Global style:

- Modern cultivation academy plus summoned-beast progression fantasy.
- High-end anime fantasy key visual.
- Cinematic lighting, readable silhouettes.
- Use the character profile images for identity consistency.
- No random extra named characters in scene images.
- Avoid text, labels, and watermarks unless a stat card is explicitly required.

Key motifs:

- Chenlin: black/silver armor in later forms, purple energy accents, calm serious expression.
- Hey Ming: black wolf/demon-wolf forms, black flame, gold markings in final forms, huge scale contrast.
- Diana: sacred gold in child/support forms; gold/silver/crimson Sun-Moon Judgment in final form.
- Silver Butterfly: polished silver, scarlet accents, living armor and blade transformations.
- System/stat cards: translucent blue-black, glowing white text, rank badges, attribute grids.
- Fallen Clan/cultists: violet, ash-black, corrupted red, bone-mask motifs.

## Location Bible Use

Before generating a scene, check `location-bible.md` for the scene location. It defines environment, lighting, props, and mood.

Important locations include:

- `Chenlin's Rented Room`
- `Second High Awakening Hall`
- `Entrance Exam Plaza`
- `Burial Bone Forest`
- `Goblin Mountain Cave`
- `Entrance Exam Viewing Gallery`
- `Second High Reception Room`
- `Yunk Academy Classroom`
- `Yunk Academy Summoning Room`
- `Yunk Academy Resource Chamber`
- `Ruined Disaster World`
- `Ruined Disaster City Streets`
- `Disaster Matriarch Core Nest`
- `Yunk Academy Dormitory`
- `Hangdon Base Mountain Range`
- `Blood Marsh Ravine`
- `Rock Drake Canyon`
- `Humanity Command Center`
- `Border Defense Ruins`
- `Border Defense Ruins Sky`
- `Balian Mountain Range`
- `Wooan Base Airstrip`
- `Wooan Base Logistics Warehouse`
- `Wooan Base Command Center`
- `Wooan Mountain Battlefield`
- `Wooan Mountain Battlefield Sky`
- `Sacred Realm Floating Island`
- `Yunk Academy Front Gate`

## Current Validation Status

The project was audited before this handoff file was created:

- `completed-rewritten-narration-story.md`
  - **10,143 words**
  - **58,643 characters**
  - **858 lines**

- `scenebreakdown.json`
  - **204 total scenes**
  - **59 first-five-minute hook scenes**
  - **89 first-ten-minute dense opening scenes**
  - **90 stat/card/evolution scenes**
  - No duplicate scene IDs.
  - Required scene fields are present.
  - Character refs are complete.
  - Every referenced profile image exists.
  - All **82 PNG profile variants** are used at least once.

- `location-bible.md`
  - Covers all scene locations after adding `Wooan Base Command Center`.

## Suggested Next Steps

The next account/chat should continue from image generation:

1. Open `scenebreakdown.json`.
2. Confirm `scene_images\scene_001_F5_001.png` through `scene_images\scene_059_F5_060.png` exist.
3. Generate scene 60:
   - output path: `scene_images\scene_060_T10_091.png`
   - scene ID: `T10_091`
   - title: `Quiet Bond: Chenlin sits beside Hey Ming`
4. Continue sequentially through all 204 scenes.
5. Periodically audit:
   - generated image count matches scene count generated so far
   - filenames are sequential
   - profile references were used
   - scenes still follow the same plot order
6. If a scene image is poor, regenerate as `scene_###_<sceneID>_v2.png` and keep the original unless the user asks to delete it.

## Exact Next Scene To Generate

The next scene is the sixtieth item in `scenebreakdown.json`.

```json
{
  "id": "T10_091",
  "title": "Quiet Bond: Chenlin sits beside Hey Ming",
  "storyMoment": "Chenlin sits beside Hey Ming",
  "location": "Chenlin's Rented Room",
  "cameraViewType": "warm closeup",
  "requiredCharacters": [
    {
      "name": "Chenlin",
      "profileImage": "Chenlin_CL-F1.png",
      "role": "newly empowered summoner"
    },
    {
      "name": "Hey Ming",
      "profileImage": "Hey_Ming_HM-F1.png",
      "role": "young wolf growth form"
    }
  ],
  "statCardRequired": false,
  "statCardReason": "",
  "imagePromptNotes": "First 10 minutes: use 4-6 second visual cadence; keep continuity with the completed rewritten story."
}
```

### Ready Prompt For Scene 60

Use this prompt as the starting point for `scene_images\scene_060_T10_091.png`:

```text
Use case: illustration-story
Asset type: 16:9 cinematic scene image for scene T10_091, save-worthy production still
Primary request: Show Chenlin sitting quietly beside Hey Ming after the first feeding and power feedback.
Input images used as character reference: Chenlin_CL-F1.png for newly empowered Chenlin and Hey_Ming_HM-F1.png for Hey Ming's young wolf growth form; preserve Chenlin's worn poor-student clothing, sharper empowered presence, and Hey Ming's black wolf identity.
Scene/backdrop: Chenlin's Rented Room, cramped poor room with old wooden floor, warm lamplight, meat bundles, scratched floorboards, and black-violet devouring energy overtaking the space.
Subject: Chenlin sits on the floor beside the young black wolf, both exhausted but calm after the impossible first growth. The image should feel intimate and quiet, with the room still marked by scratches, scattered meat remnants, and fading black-violet energy.
Style/medium: high-end anime fantasy key visual, cinematic painterly concept art, no comic panels.
Composition/framing: warm closeup in a 16:9 landscape frame; frame Chenlin and Hey Ming close together, emphasizing trust, fatigue, and the bond before the next evolution prompt.
Lighting/mood: quiet, intimate, relieved, secretive; warm single-lamp room lighting with faint cold violet-black energy fading around the floorboards.
Color palette: warm amber browns, black, deep violet, smoky indigo, faint gold accents if useful.
Constraints: preserve Chenlin and Hey Ming's design continuity from the profile references; no text, no watermark, no labels, no readable UI.
```

## Prompts Already Used For Generated Images

These are useful for matching style and continuity.

### Prompt Continuity Note

- Generated images now cover the first 59 current scenes, ending at `scene_059_F5_060.png`.
- Match the established output style in `scene_images\scene_001_F5_001.png` through `scene_images\scene_059_F5_060.png` before continuing.

## Important Don'ts

- Do not delete or rename the PNG profile files.
- Do not overwrite existing generated scene images unless explicitly asked.
- Do not remove the cold open from the story; it was intentionally added to hook the audience.
- Do not shrink the first five minutes back to macro scenes; the user requested 4-6 second image beats there.
- Do not introduce new major characters unless the user asks.
- Do not claim the final ending is from the original transcript; it is an original completion based on the project setup.
- Do not leave generated project assets only in Codex's default generated-images directory; copy them into `scene_images`.

## Quick Command Audits For Future AI

Run these from the project folder to check health:

```powershell
node -e "const fs=require('fs'); const j=JSON.parse(fs.readFileSync('scenebreakdown.json','utf8')); const ids=j.scenes.map(s=>s.id); const dup=ids.filter((id,i)=>ids.indexOf(id)!==i); console.log({sceneCount:j.scenes.length, duplicates:dup.length, statCards:j.scenes.filter(s=>s.statCardRequired).length});"
```

```powershell
$json = Get-Content -Raw .\scenebreakdown.json | ConvertFrom-Json
$files = Get-ChildItem -File -Filter *.png | Select-Object -ExpandProperty Name
$used = @{}
$missing = @()
foreach ($s in $json.scenes) {
  foreach ($c in $s.requiredCharacters) {
    if (-not $c.name -or -not $c.profileImage -or -not $c.role) {
      $missing += "$($s.id): incomplete character object"
      continue
    }
    $used[$c.profileImage] = $true
    if ($files -notcontains $c.profileImage) {
      $missing += "$($s.id): $($c.profileImage)"
    }
  }
}
$unused = $files | Where-Object { -not $used.ContainsKey($_) }
if ($missing.Count -or $unused.Count) {
  "missing/incomplete refs:"
  $missing
  "unused pngs:"
  $unused
} else {
  "all character refs complete, all referenced images exist, all PNG profile variants are used"
}
```

```powershell
Get-ChildItem .\scene_images -File -Filter scene_*.png | Sort-Object Name | Select-Object Name,Length
```

## Final Current State

The project is ready to continue scene image generation. The next concrete action is to generate `scene_060_T10_091.png` from `T10_091` in `scenebreakdown.json`, using these profiles:

- `Chenlin_CL-F1.png`
- `Hey_Ming_HM-F1.png`
