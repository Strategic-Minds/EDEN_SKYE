# EDEN SKYE PROMPT GOVERNANCE

Version: 1.0.0
Owner: Jeremy
Status: Documentation-only prompt governance
Production Impact: None

## Purpose

Defines how Eden Skye prompts are created, versioned, approved, scored, and reused across image, video, voice, chat, social, website, and product workflows.

## Authority

1. docs/EDEN_SKYE_VISUAL_IDENTITY.md
2. docs/EDEN_SKYE_AVATAR_PRODUCTION_PIPELINE.md
3. docs/EDEN_SKYE_BRAND_BIBLE.md
4. docs/collections/COLLECTION_REGISTRY.md
5. docs/auto_builder/EDEN_SKYE_RUNTIME.md

## Governance Rule

Auto Builder governs. GPT_WORKBOOK_LIBRARY informs. EDEN_SKYE executes.

## Prompt Storage

Prompt docs should live in:

- docs/prompts/
- prompts/image/
- prompts/video/
- prompts/voice/
- prompts/chat/

## Prompt Naming Format

eden_[collection]_[look]_[use_case]_v###.md

Examples:

- eden_park_no_glasses_dog_walk_v001.md
- eden_executive_glasses_library_v001.md
- eden_rooftop_no_glasses_golden_hour_v001.md

## Required Prompt Sections

Each prompt must include:

- collection
- canonical look
- reference tier
- wardrobe
- environment
- lighting
- camera language
- identity lock clause
- negative prompt
- approval threshold
- version
- intended platform

## Canonical Looks

1. No-glasses luxury/lifestyle Eden
2. Executive Eden with black rectangular glasses

Both looks must preserve the same face, hair, skin tone, eye family, and adult identity.

## Consistency Enforcement

Every prompt must include:

- same Eden face identity
- long dark brunette wavy hair
- warm olive/tan skin
- brown/hazel eyes
- soft glam makeup
- adult female presentation
- luxury editorial realism

## Negative Prompt Rules

Exclude:

- different face
- changed ethnicity or skin tone family
- blonde/red/fantasy hair
- blue/green unnatural eyes
- teen-coded appearance
- celebrity likeness
- real-person resemblance
- distorted hands
- distorted anatomy
- plastic skin
- cartoon/anime/illustration unless requested
- low-quality lighting
- off-brand wardrobe

## Scoring Rules

Use the 0-100 identity scoring system from EDEN_SKYE_VISUAL_IDENTITY.md.

Minimum thresholds:

- Public social: 85+
- Website hero: 90+
- Product imagery: 92+
- Face reference: 95+
- Video source frame: 90+

## Versioning

Increment prompt version when:

- face consistency improves
- wardrobe changes
- lighting changes
- collection changes
- negative prompt improves
- platform target changes

## Approval Flow

Draft -> Test -> Score -> Revise -> Approve -> Save -> Reuse -> Improve

## Final Rule

A prompt is only successful if the output looks unmistakably like Eden Skye.
