# Excalidraw → PDF — Evaluation guide

Start with the smallest path that exercises the project. Distinguish source inspection,
syntax/build checks, functional behavior and domain validation when recording a result.

## Guided reading and demonstration

1. **Inspect tracked contents.** The repository contains documentation only. There is no source
entry point or installable exporter.

2. **Identify absent contracts.** Input formats, rendering fidelity, PDF options and error
behavior have not been established by code.

3. **Avoid assumed installation.** There is no dependency manifest, CLI or executable test to run.
A repository clone does not provide conversion capability.

4. **Define the first evidence.** A future implementation would need a known input/output case and
documented limitations before claiming export support. That is proposed work, not a committed
feature.

## Declared checks

No executable implementation is supplied, so there is no functional check to run.

## Evidence levels

| Level | What it establishes | What it does not establish |
| --- | --- | --- |
| Source review | A path exists in tracked code | Successful runtime behavior |
| Syntax/build | Parser/compiler accepts that path | End-to-end correctness |
| Behavioral check | A specific input/output case passed | Generalization beyond cases |
| Domain evaluation | Performance on a stated target setting | Other users/data/environments |

## What to record

- Commit, environment, dependency versions and date.
- Input provenance and whether data is synthetic, public or privately supplied.
- Absolute pass/fail/skip counts; keep failed cases and their root causes.
- Whether external services, hardware or a production deployment were actually exercised.
- Expected output and an artifact showing the observation.

## Review scenarios

- **Empty state is explicit:** A name is not an implementation claim.

- **No invented commands:** Setup instructions require a real entry point and dependencies.

- **Proposed work is labeled:** Future acceptance criteria do not imply delivered functionality.

## Documentation inspection — 7 October 2026

The documentation was traced to committed source and checked for local links, balanced
code fences and supported implementation claims. Historical notebook outputs remain labeled
as historical. Live provider access, private databases and hardware behavior are not inferred
from configuration or dependency files. Any fresh run is recorded separately in the README.

## Next evidence to collect

- Choose and document the intended input contract.
- Implement one rendering/export path.
- Add a reproducible input/PDF comparison before advertising support.
