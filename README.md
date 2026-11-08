# Stage-Based Versioning (SBV)

**Stage-Based Versioning (SBV)** is a software versioning scheme that describes the maturity, stability, and maintenance status of a project through numbered development stages.

SBV consists of six stages, each represented by a name and a corresponding major version number.

## Stages

| Stage | Version | Description |
|---|---|---|
| Concept | `0-x` (`0.x`) | Concept phase. Documentation and planning only; implementation may not exist yet. |
| Alpha | `alpha-x` (`1.x`) | Active development. Frequent updates, unfinished features, and potentially unimplemented parts. |
| Beta | `beta-x` (`2.x`) | Advanced development. Frequent updates that may introduce significant changes, including syntax, APIs, CLI commands, and other core functionality. |
| Gamma | `gamma-x` (`3.x`) | Stable release. The specification is locked in, the core functionality is considered stable, and the software is generally production-ready. |
| Delta | `delta-x` (`4.x`) | Maintenance phase. Limited updates, primarily security patches and small bug fixes. Typically used for older, less-prioritized, or largely superseded software. |
| Epsilon | `epsilon-x` (`5.x`) | Discontinued software. No longer actively maintained or receiving regular updates. The software is considered deprecated or abandoned. |

## Version numbering

Each stage has its own sequential version numbering.

For example:

- `alpha-1` — first alpha release.
- `alpha-2` — second alpha release.
- `beta-1` — first beta release.
- `gamma-1` — first stable release.
- `delta-1` — first maintenance release.
- `epsilon-1` — first discontinued release.

The numerical representation can also be used:

| SBV notation | Numerical notation |
|---|---|
| `alpha-1` | `1.1` |
| `beta-1` | `2.1` |
| `gamma-1` | `3.1` |
| `delta-1` | `4.1` |
| `epsilon-1` | `5.1` |

The stage determines the major version number, while the number after the hyphen determines the release within that stage.

## Progression

The typical progression of a project is:

```text
0-x
  ↓
alpha-x
  ↓
beta-x
  ↓
gamma-x
  ↓
delta-x
  ↓
epsilon-x
```

Not every project needs to follow every stage. A project may skip stages when appropriate, and its stage may change depending on its development status.

## Philosophy

SBV aims to make software maturity immediately understandable through version numbers.

Rather than simply indicating how many releases a project has had, SBV communicates what users and developers can expect from the software, including its stability, compatibility, and maintenance status.