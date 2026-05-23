# Product Notes: Teaching with CoCalc-AI

## Useful positioning

- CoCalc is a live computational classroom, not merely an LMS.
- The strongest comparison is not "CoCalc vs Canvas"; it is "Canvas for the
  institution-facing course shell, CoCalc for the live technical work."
- The central object is a student project, not a submitted file.
- Assignment movement is operational: assign, collect, grade, return.
- Realtime instructor access is a major differentiator, but phrase it as help
  at the right moment rather than monitoring.
- TimeTravel, snapshots, and backups make student work safer and more
  inspectable.
- RootFS management is important for courses because setup problems are often
  the hidden tax in computational teaching.

## Product hooks that may deserve deeper docs

- How the collaborative `.course` file is represented and synced.
- Exact student/instructor permission model for opening student projects.
- What a student can and cannot delete, especially around snapshots/backups.
- Best practice for pairing CoCalc with an institutional LMS.
- A short recipe for a first notebook-based assignment with nbgrader.
- A short recipe for a research-style workshop with a custom RootFS.

## Claims to keep precise

- CoCalc supports peer grading, but instructors still explicitly collect graded
  peer assignments.
- nbgrader behavior depends on course settings, hidden-test settings, grading
  project choice, and time/output limits.
- Student project RootFS settings apply to new projects by default; changing
  existing projects is an explicit instructor action.
