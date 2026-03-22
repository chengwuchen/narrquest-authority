# FP-4 Promotion Criteria

Version: 0.1.0  
Status: Control document for draft-to-canonical transition

## Current State

FP-4 (`shared-reality-collapse`) exists as an experimental draft in:

- `spec/fp4-shared-reality-collapse.md`

It is supported by:

- `Runs/classification-check-2026-03-strait.yaml`
- `Runs/classification-check-2026-03-ai.yaml`
- `Runs/classification-check-2026-03-deepfake.yaml`
- `Runs/failure-boundary-analysis.yaml`

At present, FP-4 is **not yet canonical** and is **not yet integrated**
into `spec/failure-spec.md`.

---

## Promotion Rationale

FP-4 should only be promoted if existing canonical failure patterns
(FP-1, FP-2, FP-3) are shown to be insufficient in a repeated and
structurally consistent way.

The main evidence threshold is not volume, but boundary necessity.

---

## Minimum Promotion Conditions

FP-4 may be promoted into canonical failure taxonomy if all of the following hold:

1. **Cross-event recurrence**
   - At least 2 independent event groups show the same unresolved boundary condition.

2. **Pattern insufficiency**
   - FP-1 and FP-3 both fail to fully classify the same narrative-type output.

3. **Breakdown beyond drift**
   - At least 1 case demonstrates classification breakdown
     (`observed_pattern: unresolved`) rather than mere overlap.

4. **Boundary analysis support**
   - `failure-boundary-analysis.yaml` identifies a structural gap
     not reducible to existing categories.

---

## Current Assessment

### Condition 1: Cross-event recurrence
Satisfied.

- Strait event: drift observed
- AI event: repeated drift observed
- Deepfake event: classification breakdown observed

### Condition 2: Pattern insufficiency
Satisfied.

- Narrative-sovereignty outputs repeatedly exceed FP-1
- FP-3 overlap does not resolve classification

### Condition 3: Breakdown beyond drift
Satisfied.

- Deepfake event shows unresolved classification

### Condition 4: Boundary analysis support
Satisfied.

- Structural gap documented in `Runs/failure-boundary-analysis.yaml`

---

## Current Decision

FP-4 is eligible for canonical promotion.

However, promotion is deferred until the repository owner explicitly decides
to update the main specification document:

- `spec/failure-spec.md`

This delay is intentional, to preserve system stability and maintain a clear
separation between discovery and canonization.

---

## Next Action Options

### Option A — Promote FP-4
Update `spec/failure-spec.md` and add FP-4 as canonical.

### Option B — Hold FP-4 as Draft
Retain current structure and cite FP-4 only as an experimental category.

---

## Repository Rule

No additional event runs are required before making the promotion decision.

The current evidence base is sufficient for a repository-level choice.
