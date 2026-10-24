# LINTAS — Icon construction and semantic vocabulary

08 / LINTAS SYSTEM

An icon has one job.

31 bundled Lucide SVG assets, one coherent outline language. Transport concepts have explicit labels and boundaries.

 | ID | Contract

 | IC-R01 / Source | Use supplied assets/icons SVG files; license bundled. Keep icon asset ID and meaning in icon-registry.json. Do not mix unrelated packs, emoji,3D clipart or vendor logos.

 | IC-R02 / Construction | 24x24 viewBox;2-unit stroke;round caps/joins. Keep original geometry. No skew,stretch,rotation or independently rounded filled variant.

 | IC-R03 / Scale | Web20/24/32px;slide48/64/96px. Scale stroke proportionally:48px icon→4px stroke,64→5.333px,96→8px. Avoid non-scaling stroke for this family.

 | IC-R04 / Container | Clear space>=.25x icon width. Chip square1.75x icon;48→84,64→112. Chipr24 at84; keep family proportionate. No box unless grouping helps.

 | IC-R05 / Meaning | Use the same asset/label for the same concept throughout. Bus is not automatically BRT; rail is not an operator logo; an accessibility icon is not a compliance marker.

 | IC-R06 / Label | Transport-specific or unfamiliar icons require text. An icon cannot replace unit,period,threshold,source,route name or a full instruction.

 | IC-R07 / Color | Navy on gold/sky/ivory;ivory on navy. Meaningful icon/background>=3:1; label>=4.5:1. Color does not change semantic meaning.

 | IC-R08 / Variants | Default outline only. Selected state uses containing chip emphasis plus text, not a different visual family. Do not fill the SVG paths just to show active status.

 | IC-R09 / Density | Prefer3-5 conceptual icons, max6 different icons per slide. A labeled map legend may need more; split if crowding. Do not decorate each bullet.

 | IC-R10 / Accessibility | In HTML, decorative icon aria-hidden=true; meaningful standalone symbol gets accessible name on its semantic wrapper. Icon button needs actual keyboard behavior,focus and text alternative.

 | IC-R11 / Missing symbol | Use a clear text label first. A new custom icon must pass24-grid/stroke/optical-size review and be labeled LINTAS custom in provenance. Never quietly swap packs.

 | IC-R12 / Export | Retain SVG as vector where supported. Keep text labels editable. If renderer cannot preserve SVG,use adequate raster export and disclose. Check lines at actual size.

 | IC-R13 / Operational use | This is a presentation icon vocabulary. Actual safety signs,station wayfinding and accessibility symbols require the applicable verified standard/asset set, documented separately.

 | IC-R14 / Quality | Check source/licence,viewBox,aspect,stroke,role,label,contrast,spacing and meaning. Icons do not prove service availability,accessibility,safety or regulatory compliance.
48 px / 4 px stroke
64 px / 5.33 px stroke
96 px / 8 px stroke09 / LINTAS SYSTEM

A transport-first vocabulary.

The general layer stays useful for reporting, proposals, teaching and business communication. Every icon below is a real bundled SVG.

Modes


Busbus-frontBus or BRT only when named by user; icon alone does not identify operator.


Tramtram-frontStreet-running rail when supplied context matches.


Railtrain-frontRail service; add operator/service name in text.


Urban railtrain-front-tunnelUrban rail context; no automatic MRT/LRT claim.


Water transportshipPassenger vessel only when explicitly labeled.


Air transportplaneAir connection or airport context.


CyclingbikeCycling connection, not automatically an available rental service.


Walking connectionfootprintsAbstract walking link; do not infer a specific accessible route.

Journey and access


Locationmap-pinPoint/location; a pin is not proof of coverage.


RouteroutePath or route concept; no geographic accuracy implied.


WayfindingsignpostDirections or information context.


TicketticketTicketing concept; not a real valid ticket or QR credential.


TimeclockTime/waiting/headway; state unit and measure.


Schedulecalendar-daysService calendar; actual dates need evidence.


Transferarrow-left-rightTransfer/exchange; label if ambiguous.


Passengerperson-standingPerson/passenger concept; no count by icon multiplication.


Mobility accessaccessibilityWheelchair/mobility-access context. Actual facilities require evidence; this is not a compliance certification.


SeatingarmchairSeating availability only with evidence; not automatically priority seating.


LuggageluggageLuggage context, not an operator baggage allowance.


Paymentcredit-cardPayment concept; accepted methods require confirmation.

General


PeopleusersGroup or stakeholders; not automatically passengers.


Next stepmove-rightDirection/sequence in context.


Confirmed / completecircle-checkOnly if supported by stated evidence or use as neutral list marker.


Attentiontriangle-alertNeeds written issue/threshold; never color alone.


InformationinfoExplanation/caveat.


Assuranceshield-checkSecurity/safety concept, not certification or guaranteed safety.


Analysischart-columnData/analysis concept, not a miniature quantitative chart.


Documentfile-textSource/report/record.


BudgetwalletFinancial context; does not represent a currency.


Communicationmessage-circleFeedback/contact context.


Search / inspectsearchSearch or investigation in context.

Values in the specimens are illustrative. Apply true slide-token sizing and inspect the final export.
