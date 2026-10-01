# Asset Registry — Nelson Multi-Brand Automation

Status: ACTIVE — REQUIRED BY AUTOMATIONS
Owner: Nelson Rivera
Last updated: 2026-10-01

## Purpose

This registry is the mandatory source-of-truth for visual assets used by automated workflows. Every automation that creates an image, video, diagram, presentation, thumbnail, dashboard, social post, mockup, or multi-brand visual MUST resolve the correct asset before rendering.

## Hard rule

1. Resolve brand/tool ID.
2. Resolve approved asset or official vendor brand source.
3. Verify brand-to-asset mapping.
4. Generate the background/content WITHOUT recreating protected logos.
5. Composite the verified logo deterministically when possible.
6. Run final visual validation.
7. If an asset cannot be resolved, OMIT the mark. NEVER fabricate, approximate, redraw, stylize, substitute, or borrow another logo.

## Owned brand asset map

| ID | Brand | Approved reference available | Role | Automation rule |
|---|---|---|---|---|
| los-duros | Los Duros con Los Duros | YES — master logo supplied by Nelson | LOCKED MASTER | Exact approved logo only |
| scan | SCAN Water Intelligence | YES — approved SCAN logo supplied by Nelson | LOCKED MASTER | Exact approved logo only |
| zmart-consumer | Zmart Consumer Rights | YES — approved Zmart logo supplied by Nelson | LOCKED MASTER | Exact approved logo only |
| zerolag | ZeroLag WiFi | YES — approved ZeroLag branded reference supplied by Nelson | APPROVED REFERENCE | Do not invent logo; use verified asset/reference only |
| nelson-clone | Nelson Clone / Full Nelson AI | FUTURE PROJECT | NOT REQUIRED FOR CURRENT AUTOMATIONS | Do not prioritize or inject into current business workflows |
| yek-family | Yek Family | NOT RESOLVED HERE | MISSING | Text label only until approved asset is registered |
| zmart-home | Zmart Home Solutions | NOT RESOLVED HERE | MISSING | Text label only until approved asset is registered |

### Los Duros special references
- Master: official red/white/black Los Duros con Los Duros logo.
- Alternate: approved alternate master reference.
- Horizontal-layout reference: Los Duros News artwork is composition reference ONLY.
- NEVER import NEWS, Noticias en un Minuto, handles, people, portraits, or secondary artwork into the main logo.

## Paid / operational tool map

These tools must be shown only where they actually participate in a workflow. Their marks must come from the vendor's official brand source or an approved local asset — never from AI recreation.

| Tool ID | Tool | Actual role in Nelson systems | Asset policy |
|---|---|---|---|
| n8n | n8n | Primary workflow orchestration / automation engine | OFFICIAL VENDOR ASSET ONLY |
| openai | OpenAI | AI / Brain model layer where configured | OFFICIAL VENDOR ASSET ONLY |
| github | GitHub | Code, Brain rules, version control, source-of-truth | OFFICIAL VENDOR ASSET ONLY |
| highlevel | HighLevel / GoHighLevel | CRM / workflows / contacts where still in operation | OFFICIAL VENDOR ASSET ONLY |
| framer | Framer | Websites / landing pages / quiz entry points where configured | OFFICIAL VENDOR ASSET ONLY |
| meta | Meta | Ads, Facebook/Instagram integrations where configured | OFFICIAL VENDOR ASSET ONLY |
| facebook | Facebook | Comments / Messenger / Page entry channels where configured | OFFICIAL VENDOR ASSET ONLY |
| instagram | Instagram | Social/content channel where configured | OFFICIAL VENDOR ASSET ONLY |
| whatsapp | WhatsApp | Cloud API / messaging where configured | OFFICIAL VENDOR ASSET ONLY |
| gmail | Gmail | Notifications / human-review email where configured | OFFICIAL VENDOR ASSET ONLY |
| google-drive | Google Drive | Documents/evidence/files where configured | OFFICIAL VENDOR ASSET ONLY |
| muse | Muse | AI/creative intelligence workflows where actually configured | VERIFIED ASSET REQUIRED; DO NOT INVENT |

## Placement rules for automation diagrams

### n8n
Place n8n at the orchestration layer / workflow engine — not as the AI brain and not as a decorative logo.

### OpenAI
Place OpenAI only at AI/model nodes that actually call an OpenAI model. Do not use the logo as a generic AI symbol.

### GitHub
Place GitHub at source control / Brain rules / versioning / repository nodes. It is not a runtime message channel.

### HighLevel
Place HighLevel at CRM/contact/workflow nodes only where the current system actually uses it. Do not imply it owns the Brain.

### Framer
Place Framer at website/landing/quiz entry nodes when that site is the real entry point.

### Meta / Facebook / Instagram
Place each at its actual acquisition, comment, Messenger, DM, ads, or social channel node. Do not merge them into one fake icon if the distinction matters.

### WhatsApp
Place WhatsApp only on active/configured WhatsApp messaging or Cloud API nodes. Never imply an unbuilt path is live.

### Gmail
Place Gmail at email notifications/human review where configured.

### Google Drive
Place Google Drive only for actual file/document/evidence storage or retrieval.

### Muse
Place Muse only in workflows where Muse is actually used. For SCAN Creative Intelligence, it belongs in creative/competitive intelligence analysis, not as a generic database or CRM.

## Current priority

The current automation infrastructure and paid/operational tools take priority. Nelson Clone is a future project and must not be injected into current business diagrams unless Nelson explicitly requests it.

## Automation enforcement contract

Every automated visual workflow MUST include:

PRE-RENDER ASSET RESOLVER
→ BRAND/TOOL ID VALIDATION
→ VERIFIED ASSET MAP
→ GENERATION WITHOUT FAKE LOGOS
→ DETERMINISTIC LOGO COMPOSITING
→ POST-RENDER BRAND VALIDATOR
→ PASS / REJECT

Reject the output if:
- a logo was generated by the image model;
- a logo is assigned to the wrong brand/tool;
- an official mark is distorted or materially altered;
- a missing logo was replaced with an invented mark;
- an inactive/unconfigured tool is shown as active;
- a future project is presented as current infrastructure;
- the same brand logo is duplicated unnecessarily.

## Source policy

For owned brands, Nelson-approved assets override all generated references.

For third-party tools, use the vendor's official brand/press kit or a locally stored approved copy. Never scrape a random third-party logo and never ask the image model to recreate one.

Status: ACTIVE — HARD GATE
