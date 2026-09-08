# Project Engineering Values

This project strictly adheres to the core engineering values defined in **`company-core/VALUES.md`**:

1. **Simple**: Eliminate accidental complexity. No unnecessary abstractions.
2. **Professional**: Strict type safety, deterministic error handling, zero unhandled errors.
3. **Clean**: Self-documenting code, feature-first colocation.
4. **Show, Don't Tell**: Concrete examples over abstract documentation.

---

## Project-Specific Overrides & Context

*Document any project-specific constraints, performance budgets, or exceptions to standard company rules below:*

- **Performance Budget**: Target maximum bundle size: `< 150kb` initial JS.
- **Client Latency Target**: Sub-100ms response time for core user flows.
- **Security / Compliance**: [e.g. End-to-end encryption / GDPR compliance requirements]
