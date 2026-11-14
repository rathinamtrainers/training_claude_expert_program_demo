# Delivery plan — Meridian rollout

**The standing reference.** This is the document the weekly status report is always written
against, so it goes into the Project's Context beside last week's report. Invented, like
everything else in this folder.

## What is being delivered

Replacing Meridian's 11-year-old warehouse stock system with the new platform, across 3
sites: Coimbatore, Hosur and Chennai.

Contract value Rs 1.4 crore. Signed 12 June 2026.

## Who is who

| Role | Name | What they decide |
|---|---|---|
| Client, operations director | Latha Narayanan | Go-live, scope changes, anything that costs money |
| Client, warehouse lead | Suresh Raman | Day-to-day acceptance at each site |
| Us, delivery manager | the author of the weekly report | Everything else |
| Hardware vendor | Trivance Systems | Scanners and the 3 site servers |

**Latha is not technical and does not want to be.** She wants the decision first, then the
reason, then what she has to do. She has been burned by a previous supplier who reported
green until the week before go-live.

## The phases

| # | Phase | Planned finish | Status |
|---|---|---|---|
| 1 | Discovery and data audit | 31 Jul 2026 | Done |
| 2 | Build and configuration | 30 Sep 2026 | Done |
| 3 | Data migration dry runs | 20 Nov 2026 | Not started |
| 4 | Integration testing | 13 Nov 2026 | In progress |
| 5 | User training | 27 Nov 2026 | Content done, delivery not started |
| 6 | Hardware install, 3 sites | 4 Dec 2026 | Blocked on vendor |
| 7 | Go-live, Coimbatore first | **11 Dec 2026** | At risk |
| 8 | Hosur and Chennai | 15 Jan 2027 | Not started |

## What is in scope, and what is not

**In scope.** Stock in and out, stock counts, the 3 warehouse layouts, the existing
barcode format, read-only reporting, and migration of 4 years of stock history.

**Not in scope, and this has been asked for twice.** Purchase ordering, supplier
invoicing, the Chennai cold-storage units, and anything on a phone. Each of those is a
change request, not a clarification.

## Standing risks

**The hardware vendor.** Trivance has not confirmed a shipping date for the remaining 40
scanners or the Hosur server. This is the only thing between us and the go-live date, and
it has been open for 3 weeks.

**Data quality in the 4-year history.** The audit found roughly 2% of rows with no valid
site code. The agreed treatment is to migrate them to a holding location rather than guess.

**Warehouse availability in December.** Peak season. Suresh has said no site work in the
last 2 weeks of December.

## The rule about dates

**Nobody states a go-live date to Latha that has not been agreed in a plan review.** The
previous supplier moved it 3 times by mail and that is why we have this rule.
