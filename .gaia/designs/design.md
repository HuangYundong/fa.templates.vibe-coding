[<< Back](../../README.md)

## Design

System architecture following iDesign architectural principles.

### Architecture Overview

**3-Layer Hierarchical Structure**:
- **Managers** (🟢): Orchestration, use case coordination
- **Engines** (🟠): Business logic, domain algorithms  
- **Data Access** (⚫): I/O operations, persistence
- **Models** (🟣): DTOs, entities, contracts

**Dependency Rules**:
- Managers → Engines, Data Access, Models
- Engines → Data Access, Models (never Managers)
- Data Access → Models only
- Models → Self-contained

### Design Documentation

| Document | Purpose |
| --- | --- |
| [Use Cases](./1-use-cases.md) | System requirements and user goals |
| [Class Diagrams](./2-class.md) | Data models and class structure |
| [Sequence Diagrams](./3-sequence.md) | Use case execution flows |
| [Frontend](./4-frontend.md) | UI/UX specifications |

### Quality Standards

**Testing**: 100% unit test coverage, integration testing, E2E validation
**Performance**: API < 200ms, Frontend LCP < 2.5s, zero build warnings
**Security**: Automated vulnerability scanning, secure coding practices
**Regression Prevention (NEW)**: Mandatory validation that all existing features continue working when new features are added

### Regression Testing Standards (NEW - MANDATORY)

**Backward Compatibility**: All new features must maintain 100% backward compatibility with existing functionality
**Test Continuity**: Complete test suite must pass after each feature implementation before proceeding to next feature
**Feature Isolation**: New features must not interfere with existing feature behavior or state management
**Performance Preservation**: New features must not degrade existing feature performance by more than 5%
**Visual Consistency**: UI changes must not unintentionally modify existing component appearance or behavior

[<< Back](../../README.md)
