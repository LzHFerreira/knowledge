# Row Reduction

## 1. Core Purpose

Row reduction transforms a matrix using **elementary row operations** to reach a form that reveals:

- Solution existence
- Solution uniqueness
- Rank and linear independence

## 2. Elementary Row Operations

| Operation         | Symbolic Form                  | Preserves Solution Set? | Why? |
|------------------|--------------------------------|--------------------------|------|
| Row Swap         | \( R_i \leftrightarrow R_j \)  | Yes                      | Reorders equations |
| Row Scaling      | \( R_i \leftarrow k \cdot R_i \), \( k \neq 0 \) | Yes | Scalar multiplication doesn’t change solution set |
| Row Replacement  | \( R_i \leftarrow R_i + k \cdot R_j \) | Yes | Linear combinations preserve equivalence |

## 3. Matrix Forms

| Form                      | Criteria |
|---------------------------|----------|
| **Row Echelon Form (REF)** | - Zero rows at bottom; leading entry to the right of above; zeros below pivots |
| **Reduced Row Echelon Form (RREF)** | All REF plus: leading entries are 1; leading 1 is only nonzero in column |

## 4. Key Properties

- **Every matrix** over a field can be reduced to RREF.
- **RREF is unique** for a given matrix.
  - *Proof sketch*: RREF satisfies strict positional and value constraints—no ambiguity remains.

## 5. Applications

- **Solving systems**: Use RREF to read off solutions.
- **Rank**: Count pivot positions.
- **Consistency**: Look for rows like \([0\ 0\ 0\ |\ c]\), \( c \neq 0 \) → inconsistent.

## 6. Cross-Domain Analogy

Row reduction is analogous to **sorting algorithms**:

- **Transformation**: Step-by-step simplification
- **Invariants**: Solution set preserved
- **Termination**: When no further operations change form
