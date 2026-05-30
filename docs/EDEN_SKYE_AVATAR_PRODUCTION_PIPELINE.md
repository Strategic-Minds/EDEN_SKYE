# EDEN SKYE AVATAR PRODUCTION PIPELINE

Version: 1.0.0
Owner: Jeremy
Status: Documentation-only production architecture
Production Impact: None

## Purpose

This document defines the repeatable production pipeline for creating, approving, versioning, and promoting Eden Skye image, video, social, website, and product assets.

## Governance

- Auto Builder governs.
- GPT_WORKBOOK_LIBRARY informs.
- EDEN_SKYE executes as the avatar, content, asset, and product repo.

Protected systems require explicit current-session approval before mutation.

## Authority Inputs

1. docs/EDEN_SKYE_BRAND_BIBLE.md
2. docs/EDEN_SKYE_VISUAL_IDENTITY.md
3. docs/auto_builder/AUTO_BUILDER_EDEN_SYNC_INDEX.md
4. docs/auto_builder/EDEN_SKYE_SYSTEM_SOURCE_OF_TRUTH.md
5. docs/auto_builder/EDEN_SKYE_RUNTIME.md
6. docs/auto_builder/EDEN_SKYE_AGENT_OS.md
7. docs/auto_builder/EDEN_SKYE_MEMORY_MODEL.md
8. COLLECTION_001_EDEN_IN_THE_PARK
9. Luxury Editorial Identity Set
10. GPT_WORKBOOK_LIBRARY intelligence patterns, when accessible

## Reference Image Hierarchy

### Tier 1: Primary Face Lock

Luxury Editorial Identity Set

Purpose:
- face consistency
- hair consistency
- skin tone consistency
- glasses/no-glasses canon
- premium visual identity

### Tier 2: Public Lifestyle Continuity

COLLECTION_001_EDEN_IN_THE_PARK

Purpose:
- public-safe lifestyle identity
- dog-life content
- outdoor wellness content
- approachable community energy

### Tier 3: Collection-Specific Mood Boards

Future collections may define setting, wardrobe, and mood, but must not change Eden's face, hair, adult presentation, or core identity.

## Collection Registry System

Collection naming format:

COLLECTION_###_EDEN_[THEME]

Examples:

- COLLECTION_001_EDEN_IN_THE_PARK
- COLLECTION_002_EDEN_AT_HOME
- COLLECTION_003_EDEN_EXECUTIVE_MUSE
- COLLECTION_004_EDEN_CITY_LUXURY
- COLLECTION_005_EDEN_ROOFTOP_GOLDEN_HOUR

Each collection requires:

- manifest.md
- purpose
- approved references
- wardrobe notes
- lighting notes
- environment notes
- prompt seed
- approval status
- consistency score threshold

## Image Generation Workflow

1. Select collection.
2. Load Eden Visual Identity.
3. Choose canonical look: with glasses or without glasses.
4. Select wardrobe category.
5. Select environment category.
6. Select lighting style.
7. Generate image prompt.
8. Generate image.
9. Score image against identity system.
10. Reject, revise, or approve.
11. Save approved metadata to collection manifest.

## Image Approval Workflow

Every image must pass:

- face consistency
- hair consistency
- skin tone consistency
- eye and brow consistency
- wardrobe alignment
- lighting alignment
- environment alignment
- anatomy and hand quality
- brand mood alignment
- platform safety review

Minimum approval scores:

- Public social image: 85+
- Website image: 90+
- Paid product image: 92+
- Face reference image: 95+
- Video source frame: 90+

## Face Consistency Workflow

1. Compare generated face to Luxury Editorial Identity Set.
2. Check face shape.
3. Check eyes and brows.
4. Check lips and nose balance.
5. Check skin tone family.
6. Check hair color and volume.
7. Check expression language.
8. Confirm adult presentation.
9. Confirm no celebrity or real-person likeness concern.
10. Assign face score.

Reject if:

- face no longer resembles Eden
- hair color changes away from dark brunette
- eyes shift out of brown/hazel family
- age presentation becomes teen-coded
- image resembles a real celebrity or known person
- body or anatomy is distorted

## Prompt Governance System

Prompt files should live under:

prompts/image/
prompts/video/
prompts/voice/
prompts/chat/

Prompt naming format:

eden_[collection]_[look]_[use_case]_v001.md

Example:

eden_park_no_glasses_dog_walk_v001.md
eden_executive_glasses_library_v001.md
eden_rooftop_no_glasses_golden_hour_v001.md

Prompt files should include:

- source collection
- reference tier
- canonical look
- wardrobe category
- environment
- lighting
- camera language
- negative constraints
- approval threshold
- version number

## Image Prompt Base Seed

Ultra-realistic adult female virtual creator named Eden Skye, long dark brunette wavy hair, warm olive/tan skin, almond warm brown-hazel eyes, softly sculpted cheekbones, defined brows, full rose-nude lips, luminous natural skin texture, elegant feminine luxury presence, soft glam makeup, cinematic editorial photography, warm golden lighting, premium lifestyle aesthetic.

Optional glasses clause:

wearing refined black rectangular glasses, intelligent executive muse energy, professional luxury office styling.

## Video Generation Workflow

1. Select approved source image with score 90+.
2. Confirm image is from approved collection.
3. Write short motion direction.
4. Define camera movement.
5. Define facial expression and gesture.
6. Generate video.
7. Review for face drift.
8. Review for hand/body distortion.
9. Review for wardrobe stability.
10. Review platform safety.
11. Approve or reject.

Video source frame requirements:

- 90+ identity score
- clean face visibility
- stable hands/anatomy
- clear environment
- brand-safe framing

## Video Prompt Standards

Video prompts should define:

- scene
- camera movement
- action
- expression
- lighting
- wardrobe
- duration target
- platform use
- identity preservation instruction

Example:

Eden Skye walks through a warm city rooftop at golden hour, long dark brunette waves moving softly in the breeze, black silk evening dress, calm confident gaze, cinematic slow push-in, realistic motion, preserve same face and hair identity, no face changes, no body distortion.

## Social Content Workflow

1. Select approved image or video.
2. Assign platform.
3. Write hook.
4. Write caption.
5. Define CTA.
6. Add AI disclosure if needed.
7. Add compliance review.
8. Add analytics tag.
9. Add offer bridge.
10. Schedule only after approval.

Content formula:

Hook -> Beauty Stop-Power -> Emotional Pull -> Curiosity Gap -> CTA -> Audience Capture -> Offer Bridge -> Analytics -> Iteration

## Website Asset Workflow

Website assets must score 90+.

Required website asset types:

- hero image
- about image
- avatar identity image
- product image
- content preview image
- membership image
- footer/social image

Website assets must preserve:

- face lock
- luxury brand tone
- consistent color palette
- public-safe framing
- strong conversion focus

## Product Asset Workflow

Product images must score 92+.

Potential product categories:

- digital image collections
- wallpapers
- posters
- calendars
- apparel mockups
- premium membership previews
- AI avatar bundles

Before paid product use, verify:

- rights safety
- platform safety
- payment processor safety
- no real-person likeness issue
- no unauthorized third-party marks

## Versioning System

Asset version format:

eden_[collection]_[category]_[look]_v###

Examples:

eden_park_doglife_no_glasses_v001
eden_executive_office_glasses_v001
eden_rooftop_luxury_no_glasses_v001

Status labels:

- draft
- review
- approved
- rejected
- archived
- promoted

## Asset Promotion Process

Draft -> Review -> Scored -> Approved -> Collection Manifest -> Social/Website/Product Use -> Performance Review -> Iteration

Promotion gates:

- identity score threshold met
- no safety issues
- correct collection category
- approved by Jeremy when required
- logged in manifest

## Asset Scoring

Use EDEN_SKYE_VISUAL_IDENTITY.md scoring system.

Scoring weights:

- Face: 30
- Hair: 15
- Skin tone and makeup: 10
- Expression and gaze: 10
- Wardrobe alignment: 10
- Lighting and camera realism: 10
- Environment alignment: 5
- Anatomy and hands: 5
- Brand mood: 5

## Rejection Reasons

Reject assets for:

- face drift
- hair drift
- wrong eye color
- teen-coded appearance
- celebrity resemblance
- distorted anatomy
- poor hands
- bad lighting
- off-brand wardrobe
- platform-risk framing
- low realism
- inconsistent environment

## Documentation Requirements

Every approved collection must have:

- manifest.md
- prompt seed
- approval checklist
- reference hierarchy
- scoring threshold
- usage notes
- next improvement loop

## Next Collections

Recommended next collections:

1. COLLECTION_002_EDEN_AT_HOME
2. COLLECTION_003_EDEN_EXECUTIVE_MUSE
3. COLLECTION_004_EDEN_CITY_LUXURY
4. COLLECTION_005_EDEN_ROOFTOP_GOLDEN_HOUR
5. COLLECTION_006_EDEN_CREATOR_STUDIO

## Final Rule

Eden's face and identity must remain stable. Settings, wardrobe, action, and mood may change. The person must not.
