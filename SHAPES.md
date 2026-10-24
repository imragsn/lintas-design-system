# LINTAS — Shape,route and image mask contracts

06 / LINTAS SYSTEM

Routes, nodes and windows.

One consistent geometry family. Distinguish decoration from diagrams with informational meaning.

 | ID | Geometry at1920x1080 | Use / limits

 | S01 / Information panel | Rectangular card,r24; padding40;gap24;minimum320x240 | Default text/KPI. One nesting level max. Small panel short side<240 usesr12.

 | S02 / Window frame | TL64 TR64 BR24 BL24; minimum400x400 | Hero/portrait photo. Center subject; text outside. For smaller frame use rTop=min(64,shortSide/6),rBottom=min(24,shortSide/10).

 | S03 / Editorial image | Rectangle,r24 or0 if source edge matters | Evidence screenshot/diagram uses contain and no destructive rounding if content lost.

 | S04 / Pill | Height56-64;r=height/2;horizontal24/vertical12 inset | Short category. Max3 per slide. Labels are not fake interactive buttons.

 | S05 / Route ribbon | Stroke48, round caps;centerline bend radius144;45/90degree turns only | Exact90-degree path example:M96 600 H528 A144 144 0 0 0 672 456 V240. One decorative ribbon max; can crop at slide edge. No marks/numbers that imply real stops. Keep outside text and plot areas.

 | S06 / Connection node | Outer112,inner64,concentric circles | Decorative connection or process node; label if meaningful. Do not imply a real station/interchange without source.

 | S07 / Process connector | Stroke4;arrowhead16x12;clearance24 | Use actual sequence and labeled branches. Keep arrow lines away from icon/text.

 | S08 / Photo strip | 2-3 equal S02/S03 crops,gap24 | Consistent ratios and focal-point audit. Photo panels carry captions; no arbitrary collage.

 | S09 / Metric cluster | 1 primary +2-3 support S01 cards | Sizes indicate relevance, not magnitude. No rounded chart bars inside rounded cards.

 | S10 / Icon chip | Icon48 within84x84 chip;r24 | Icon box1.75x icon; clearspace>=.25x icon. Gold/sky chips with navy icon.

 | S11 / Real route diagram | Stroke8;stop20;interchange two rings;consistent labels | Informational route network. Solid actual,dashed planned with legend. Use true source connectivity; mark schematic if spacing not geographic.

 | S12 / Chart container | Outer cardr24;inner plot rectangular and unclipped | Axes,bars,uncertainty and labels never masked into windows/ribbons. Bar ends square; no decorative distortion.S01Information panel / r24S02Window /64,64,24,24S05 / route ribbonS06 / connection node07 / LINTAS SYSTEM

Human context. Honest framing.

Photographs remain photographs inside non-destructive masks. Preserve original files and evidential context.

 | ID | Rule

 | M01 / Roles | Documentary evidence must be authentic supplied/licensed material. Editorial stock/illustration can establish mood but cannot stand in for an actual event, fleet condition, user endorsement or outcome.

 | M02 / Source register | Author/source URL,license or permission,filename,original dimensions,generation status,role,caption,alt text. Keep original unchanged.

 | M03 / Fit and mask | Cover for editorial photos; contain for logos,diagrams,evidence screenshots or cropped-edge-sensitive material. Default S02 window for hero, S03 for evidence. Never stretch.

 | M04 / Focal | Record normalized fx,fy in[0,1]. Inspect faces,hands,assistive devices,vehicle doors and relevant context; .5,.5 is fallback only.

 | M05 / Exact crop | For sourceW,H and framew,h: s=max(w/W,h/H);rw=sW,rh=sH;x=clamp(w/2-fx*rw,w-rw,0);y=clamp(h/2-fy*rh,h-rh,0). Place then clip; preserve metadata.

 | M06 / Example | 2400x1600→720x900,focal(.60,.45): s=.5625,rw1350,rh900,offset(-450,0);visible1280x1600. On5x6.25in placement,effective256PPI.

 | M07 / Resolution | Use13.333x7.5in slide master for print calculation. Prefer150PPI;minimum100PPI photos. Screenshots must also remain legible at final size.

 | M08 / Safe regions | Text inset48; at top rounded corners keep content clear of96x96 zones. Default caption outside, gap16-24. Do not hide accessibility features in a crop.

 | M09 / Overlays | Prefer separate solid text. Full-photo cover may use opaque navy text field/scrim after checking every text region. Avoid white text on an unverified image.

 | M10 / Cutout | Use only when relevant, with source and clean edges. Keep mobility devices and companions if meaningful. Do not synthesize evidence by adding/removing documentary objects.

 | M11 / Editable export | Native crop-to-shape if supported. If editor cannot reproduce S02,use S03r24 and disclose. Preserve original/mask metadata. Do not flatten whole slides.

 | M12 / Inclusion and QA | Reflect varied passengers respectfully. Check crop,context,resolution,contrast,caption,rights and real export. Do not infer disability or service access from appearance alone.16 / LINTAS SYSTEM

A window, not a distortion.

An original vector scene demonstrates clipping; authentic photography can use the same mask contract.

S02 / WINDOW FRAME

Keep the subject.Keep the context.

Top radius64px. Bottom radius24px. No skew or stretch. Captions and claims remain editable outside the image.

M64 0 H656 A64 64 0 0 1 720 64 V876 A24 24 0 0 1 696 900 H24 A24 24 0 0 1 0 876 V64 A64 64 0 0 1 64 0 Z

Synthetic illustration. No operator,vehicle specification or service availability is represented.17 / LINTAS SYSTEM

Connectivity has meaning.

A decorative ribbon never substitutes for an evidenced route diagram.

 | Layer | Requirements

 | Decorative | One48px ribbon, no station names or real route numbers. Lives outside data/text. Can be omitted in general decks.

 | Schematic network | Source graph and connectivity required for real use. Label schematic; consistent stops/interchanges,direction and legend. Do not infer distance/time from spacing.

 | Geographic network | Use referenced coordinates/projection,basemap licence,scale and data cutoff. Distinguish planned and operational. Coverage claims require a defined calculation.

 | Accessible journey | State verified links,facilities and conditions. A node or access icon alone does not establish step-free/end-to-end access.

 | General adaptation | Same connector/node vocabulary can show workflow or stakeholder relations; relabel it accordingly,avoid transport claims.

Values in the specimens are illustrative. Apply true slide-token sizing and inspect the final export.
