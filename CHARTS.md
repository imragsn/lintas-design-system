# LINTAS — Chart and transport metric contracts

12 / LINTAS SYSTEM

Choose the question before the chart.

Charts are evidence instruments. Every type needs a reason, a data contract and an interpretation boundary.

 | ID / question | Preferred chart | Data / restriction

 | D01 / Compare categories | Horizontal bars | Category + numeric value + unit. <=8 categories main slide; sort by value unless chronological/ordinal. Zero baseline; negative values around visible zero.

 | D02 / Compare groups | Grouped bars or dot plot | Two or three series per category; <=6 categories. Shared scale and consistent order. Do not compare unaligned floating cards.

 | D03 / Trend | Line | Ordered time + numeric measure. Up to4 series; real time spacing. Unequal intervals are not equally spaced. Label nonzero baseline and explain rationale.

 | D04 / Part-to-whole | 100% stacked bar | Exhaustive, mutually exclusive categories with denominator. Show count/sample size. Use consistent segment order, <=5 categories. Do not stack unrelated measures.

 | D05 / Simple share | Donut, optional | Only positive parts of a known whole; 2-5 segments; sum reconciles to100%. Prefer bar for precise comparisons. Ring thickness30% outer radius; no exploding segments.

 | D06 / Distribution | Histogram or dot plot | Raw observations or documented bins. Label bin boundaries and counts; compare same bins, include zero count bins. Never smooth away outliers.

 | D07 / Relationship | Scatter | Paired x/y records with units; same record per point. Correlation does not prove cause. Never invent a trend fit; disclose sample/fit method.

 | D08 / Actual vs target | Bullet / paired dots | Actual, target, period and explicit benchmark definition. Target marker labeled; qualitative bands only with approved thresholds.

 | D09 / Change contribution | Waterfall | Opening balance, signed additive changes, closing balance. Opening + changes = closing; show connector, signed labels and total vs delta encoding.

 | D10 / Many comparisons | Heatmap | Row/column numeric matrix with known scale. Sequential darkening for magnitude; diverging scale only with meaningful midpoint. Values/legend required; missing has distinct pattern.

 | D11 / Uncertainty | Range / interval plot | Center + lower/upper bound, confidence level or range definition if supplied. Distinguish prediction from confidence interval. Never manufacture uncertainty.

 | D12 / Flow | Process diagram, or Sankey if true quantities | A simple arrow is not a quantitative flow. Sankey requires conserved quantities and compatible units; audit nodes before use.

 | D13 / Exact lookup | Table | When precise values, long labels or mixed measures matter more than pattern. Right-align numbers, include units and source.

 | D14 / Geography | Map only if geography matters | Use rates for choropleth; raw counts may require proportional symbols. Publish denominator/class bins; do not infer impact from land area.13 / LINTAS SYSTEM

Chart anatomy, without ambiguity.

All chart units below refer to a 1920 x 1080 slide. Smaller previews are scaled illustrations.

 | Contract | Specification

 | D15 / Frame | Minimum plot760 x360; recommended evidence region1100 x560. Title and takeaway outside plot. Reserve left144/right48/top72/bottom96 initially; increase for labels rather than reduce type.

 | D16 / Text | Read label26 px, Present30 px; chart heading44 px; explanatory copy30/36. Units in axis title or title; no unexplained K/M abbreviations.

 | D17 / Axes | 4-6 major ticks, human-readable intervals1/2/2.5/5 x10^n. Grid1 px line token, zero axis2 px navy; meaningful series>=3:1. Numeric baseline and any breaks explicit.

 | D18 / Marks | Line5 px; markers14 px; bar max width112 px; inner gap40% of bar width as starting point. Bars square-ended. Focus pale fill outlined2 px navy. No shadows/gradient/3D on values.

 | D19 / Category encoding | Use fixed semantic series mapping across deck; same category always same color/marker. Dark series palette supports five; line max4. Gold is a highlight, not a new category by default.

 | D20 / Direct labels | Label at line ends with >=16 px separation and24 px plot clearance. Resolve collisions by expanding or splitting; do not overlap or hide values. Legend if needed in reading order, not color order.

 | D21 / Formatting | Consistent precision/unit; right-align decimals in tables. Locale follows user. Distinguish percentage change from percentage points. Negative sign not only red; estimated value explicitly labeled.

 | D22 / Missing | Missing is null;0 is real zero. Break lines at null, no silent interpolation. For heatmap use hatch/Not available; for bar show Not available outside axis rather than zero-width bar.

 | D23 / States | Actual solid; target dashed + label; forecast dashed + label and boundary date. Confidence band only from provided bounds. Patterns supplement color; no invented status thresholds.

 | D24 / Focus | One primary highlight per chart, at most2 callouts. Label reason for highlighting. Keep decoration outside plot; do not crop axes/intervals to rounded or diagonal mask.

 | D25 / Integrity | Shared scales for comparable panels. No dual axes by default; separate aligned plots. No truncated bar axis, area/volume distortion, stock icons scaled as values or arbitrary pie perspective.

 | D26 / Alternatives | Provide underlying data table and a concise accessible summary. HTML SVG requires title/desc; PDF reading order and selectable labels checked where supported.

 | D27 / Source | Source locator, period/cutoff, denominator, transformation and caveat adjacent. Labels actual/target/forecast/illustrative must survive export.

 | D28 / QA | Recompute totals/deltas/percentages. Test sign, rounding, sample size, null vs0, axis/domain, intervals, label collisions, category mapping, focus and source. Inspect actual export.

Chart record:
chartId · question · chartType · datasetId · sourceLocator
period/cutoff · units · denominator · fields/types · missingPolicy
transformation · domain/baseline · ticks · seriesMapping
labels · focusReason · caveat · accessibleSummary · exportQA14 / LINTAS SYSTEM

Define the service measure.

A transport chart needs the same evidence discipline as any other chart, plus operational definitions.

 | ID / measure | Required definition / correct use

 | TR01 / Ridership | Boardings,trips,ticket validations and unique people are different measures. State which is counted,coverage,period and source. An interchange may count twice in boardings.

 | TR02 / Punctuality | On-time definition/tolerance,scheduled or operated denominator,cancelled-trip treatment,location and period. No assumed universal threshold. Example88/100=88% only under stated fictional definition.

 | TR03 / Headway | Time between consecutive departures/arrivals at same point/direction/time window. Show planned vs observed and variability. Mean alone can hide bunching.

 | TR04 / Waiting | Observed waiting vs modeled estimate. Half-headway is an estimate only under stated assumptions; irregular services need a justified model.

 | TR05 / Occupancy | Passengers divided by stated seats/capacity; distinguish seating occupancy from load factor using total capacity. State point/segment/period. Example50/80 seats=62.5% seated occupancy.

 | TR06 / Coverage | Population,area,stops or route-km denominator; buffer/walk-network definition and data cutoff. Coverage is not automatically accessibility or usability.

 | TR07 / Reliability | State cancelled/operated/scheduled measures separately; avoid comparing metrics with different denominators. Show planned vs actual service.

 | TR08 / Transfers | Transfer count,time,walking distance/fare and source. Schematic network shows connectivity,not proven travel times or geographic distance.

 | TR09 / Mode share | Mutually exclusive trip categories,period,geography and survey/source denominator. Round only after computing; reconcile to100% or explain missing coverage.

 | TR10 / Accessibility | Describe verified features/service conditions. An icon or photograph alone does not establish end-to-end accessible travel.

 | TR11 / Safety | Counts need exposure basis for fair rate comparisons,period and definitions. No unsupported safety ranking or inference from a shield icon.

 | TR12 / Planned service | Explicitly label planned/proposed/under construction. Future route or fleet symbols cannot be styled as verified operational availability.

Illustrative headways6,8,10,8 minutes have mean8 and population standard deviation1.414 minutes (CV17.68%). This example demonstrates that a mean can match a plan while intervals still vary; it is not a service assessment.15 / LINTAS SYSTEM

Six ways to show the evidence.

Rendered from example-data.json. These generic analytical patterns are available across domains; transport-specific metric definitions are documented above. No real organization, outcome or source dataset is implied.ILLUSTRATIVE DATA

Comparison, on one scale.

Bar lengths encode value; C is the focal category.

D01 / Square-ended bars; common baseline; gold outlined in navy.ILLUSTRATIVE DATA

A gap is not zero.

Q3 has no actual value; the actual line stays broken.

D03 / D22 / No inferred trend across missing observations.ILLUSTRATIVE DATA

A defined whole.

A donut is optional; use bars when precision matters.

D05 / Actual data sums to100%; exact values remain visible.ILLUSTRATIVE DATA

Contributions reconcile.

Opening and closing totals differ from signed changes.

D09 / Signed changes, total bars and connectors; additive reconciliation checked.ILLUSTRATIVE DATA

Relationship, not causation.

Paired observations; no invented fit or causal claim.

D07 / Five observations; no generated regression line.ILLUSTRATIVE DATA

Magnitude and missingness.

Sequential bins; absent value has a distinct hatch.

D10 / Values remain explicit. Hatch is reserved for missing data.

 | Underlying sample | Values

 | Bars / points | A40,B65,C80; scale0–100

 | Trend / points | Q1 28,Q2 42,Q3 null,Q4 60; target40; scale0–80

 | Shares / percent | A45,B30,C25; total100%

 | Waterfall / units | 100+25−15+10=120

 | Scatter / x,y | (2,3),(4,4),(5,2),(7,6),(8,5)

 | Heatmap / scores | R1[20,40,null];R2[60,80,100]; scale0–100

Values in the specimens are illustrative. Apply true slide-token sizing and inspect the final export.
