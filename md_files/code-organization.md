## Code Organization

Keep the repository modular. Do not keep adding new logic to one large file.

Before writing new code:
- search for existing implementations first;
- reuse existing functions, classes, modules, and config patterns when possible;
- extend or refactor existing code instead of creating near-duplicate code.

Entry-point scripts should stay thin. Put reusable logic in modules, not in scripts.

When adding code, place it in the most appropriate existing module. If no appropriate module exists, create a small focused module with a clear responsibility.

Avoid duplicating:
- data loading / preprocessing;
- model construction;
- training or evaluation loops;
- metrics;
- checkpointing;
- logging;
- visualization/debug utilities.

If the requested change would make a file too large or mix unrelated responsibilities, do a small refactor first, then implement the change.

In the final response, mention what existing code was reused and where new logic was placed.
