# Changelog

All notable changes to MediaPilot will be documented in this file.

## Unreleased

### Added

- Added video listing support for `.mp4`, `.webm`, `.mov`, `.m4v`, `.mkv`, and `.avi`.
- Added browser-native video previews in the gallery grid.
- Added video playback support in the modal viewer with native controls.
- Added `media_type` to `/images` API responses so clients can distinguish images from videos.

### Changed

- Updated gallery and modal wording from image-only language to media language where applicable.
- Updated README to mention video support.
- Bulk upscale now ignores video files and reports that upscale only supports images.

### Notes

- No dependency changes were required. Video support uses browser playback and existing static file serving.
- Video preview depends on browser codec support.
- Video poster thumbnail generation is not included yet.
- Metadata search remains image-metadata based.
