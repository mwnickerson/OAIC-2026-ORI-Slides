# Seed and environment generation

Reference [12] for slide 19. This explanation was checked against generator and task-compilation source at revision `0f0eaa8e10f65c897c2a07f03033a31b874e5a01`. It is a source audit, not a new benchmark or full regeneration test.

## What the seed controls

Seed 67 has no special meaning: it initializes repeatable pseudorandom choices. For the complex benchmark profile, identity and size use separate seeded streams. The identity stream `seeded-benchmark-v1:complex:67:identity` selects a company prefix, suffix, and domain ending from fixed lists. A separate stream chooses base counts within 4,500–5,500 users, 1,750–2,250 workstations, and 400–600 servers. These are base generation ranges, not guaranteed final node counts; templates and other construction steps can add entities.

The name generator and graph RNG are seeded too. Graph choices include the domain SID and eligible users/computers filling attack-path roles. Templates prescribe the scenarios; departments and built-in groups include fixed structure. Changing the seed therefore need not change every graph element.

## Environment first; questions separately

The generator writes a BloodHound-compatible ZIP and manifest. Task compilation separately binds question templates to entities and facts from that environment. The seed changes inputs to those bindings; it does not select question templates or control model sampling. Repeating seed 67 is not a test of multiple environments.

Repeatability requires a pinned generator version, profile and settings as well as the seed. The complex-generation path normalizes timestamps after planting paths; intermediate clock reads alone are not evidence of changing final complex output. JSON normalization and fixed archive timestamps are distinct concerns. No claim of a freshly executed, byte-identical full regeneration is made here.

## Audit anchors

Repository-relative paths identify the inspected source without publishing source modules or private filesystem paths. Public accessibility of the upstream code revision was not verified.

- `src/ori/generator/benchmark_profiles.py:91` — identity/scale streams and profile ranges.
- `src/ori/generator/graph.py:167` — seeded graph RNG and SID construction.
- `src/ori/generator/org.py:11–45` — fixed organizational structure and seeded names.
- `src/ori/generator/templates/complex_multihop.py:818–840` — eligible entity selection for a prescribed path.
- `src/ori/generator/phase4.py:13–56` and `src/ori/generator/templates/phase4.py:7–32` — complex build and timestamp normalization.
- `src/ori/generator/serializer.py:57–65,138–147` — archive serialization.
- `src/ori/eval/tasks.py:701–723` and `src/ori/eval/v2/compiler.py:2455–2532` — separate task generation and binding.

The audit compared the relevant source with the pinned revision and used an isolated scalar PRNG example. It did not import/run ORI, generate a graph, call a model, or verify a historical campaign's graph identity. The talk's current benchmark scope remains seed 67 only.
