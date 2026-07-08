# Contribution #22419: [EPIC] Apply try_to_proto / try_from_proto pattern to ExecutionPlan

**Contribution Number:** 1
**Student:** Athul Thulasidasan
**Issue:** https://github.com/apache/datafusion/issues/22419
**Status:** Phase II

---

## Why I Chose This Issue

This issue stood out to me because it improves an important internal pattern rather than just adding one more
serialization case. Moving ExecutionPlan serialization toward the same try_to_proto / try_from_proto approach already
used for PhysicalExpr makes the code easier to extend and reduces the need to expose internal state only for protobuf
support.

It also matches what I want to practice as a contributor: making focused infrastructure changes in a large Rust
codebase without changing behavior or wire format. I’m especially interested in understanding how DataFusion handles
physical plan serialization today and helping move it toward a cleaner, more maintainable design.

---
