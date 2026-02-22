# ChatEdit AI ( `ChatEdit_AI.ds`)

## Overview
`ChatEdit_AI.ds` defines a Zoho Creator application named **ChatEdit AI** for conversational video editing workflows.  
It models video uploads, transcription, AI-driven editing commands, suggested edits, subtitles, and session tracking.

## App Configuration
- App name: `ChatEdit AI`
- Date format: `dd-MMM-yyyy`
- Time zone: `America/Los_Angeles`
- Time format: `24-hr`
- Theme customization includes Poppins font and predefined color theme options.

## Core Data Model (Forms)
1. `user_videos`  
Stores uploaded video metadata, user, media reference, status, preview URL, and duration.

2. `transcripts`  
Stores transcript text per video, language, and transcription status.

3. `transcript_segments`  
Stores timestamped transcript chunks with confidence, word count, and speech/silence marker.

4. `editing_commands`  
Captures user natural-language prompts, interpreted action, target text, timestamps, and processing status.

5. `suggested_edits`  
Stores AI-proposed edit actions (trim/remove/replace/insert), time ranges, confidence, and review/apply state.

6. `subtitles`  
Stores subtitle text, segment/video relation, timing, style attributes, and creation metadata.

7. `edit_sessions`  
Tracks session lifecycle, activity timestamps, total edits, user, and stage progression.

8. `media`  
Stores media object metadata (created/updated time, progress, status, type, description).

## Workflow Coverage
- Video upload and metadata tracking
- Transcript generation and segmentation
- Prompt-to-edit interpretation
- Suggested edit review and application tracking
- Subtitle generation and styling
- Session-based editing lifecycle management

## Reports and Views
The file includes:
- List/kanban reports for edits, videos, transcripts, commands, sessions, and media
- Grouped reports (for example by status or interpreted action)
- Conditional formatting for key statuses/action types
- Quick view/detail view layouts with related-record blocks

## Navigation
The app menu is organized into sections:
- Dashboard
- Edits
- User Videos
- Subtitles
- Editing Commands
- Transcripts
- Transcript Segments
- Edit Sessions
- Media
- App Preferences
- Approvals
- Shared Reports

## Device-Specific Settings
- Separate `phone` and `tablet` configurations
- Auto label placement on forms
- Sliding pane layout and mobile/tablet theme settings

## Notes
- The file appears to be a generated Zoho Creator DSL export.
- It includes both desktop and mobile/tablet UX configuration plus localization settings.
- Naming in this README assumes your referenced file `chatedit.ds` corresponds to `ChatEdit_AI.ds`.
