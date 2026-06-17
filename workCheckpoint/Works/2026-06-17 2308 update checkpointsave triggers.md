# Update CheckpointSave Triggers

- Updated `Skills/checkpointsave/SKILL.md`.
- Added a task-start automatic trigger that instructs the assistant to read and remember `workCheckpoint\Rules` and `workCheckpoint\Works` when workspace memory is missing or before the first important task in a session if those records have not been read.
- Renamed the previous automatic trigger section to task-end automatic trigger and kept its existing content unchanged.
