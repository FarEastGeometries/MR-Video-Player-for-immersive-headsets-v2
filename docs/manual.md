# Manual

## Known issues

- If both Motion Controller and Xbox Controller are connected, Motion Controller will not work properly.
- Click the "Open in Browser" button (Manual etc.) to open it in the desktop web browser. This issue occurs when new Microsoft Edge based on Chromium is installed. In our environment, installing "2020-01 Cumulative Update for Windows 10 (KB4532695)" solved this issue.

## Notes

- Motion Controller Model is not displayed in v2.0.1.0 or higher.
- Pointer appears only when UI is displayed.
- A copy of the video file is created in the app's temporary folder to avoid issue with stereo video files containing specific metadata not playing properly. (e.g. videos shot with VR180 cameras)  
  Edit the metadata of this copied file and use it for video playback.  
  This copied file will be deleted when you open another file.
- Symbolic links cannot be handled by App-specific file picker added in v2.  
  If you use symbolic links, use the Windows file picker (file selection method used in v1).  
  Switching between App-specific file picker and Windows file picker was added in v2.2.0.0.

## Features

- Support 180°/360° equirectangular projection videos and photos
- Support 180° fisheye projection videos and photos  
  Supported fisheye projection  
  - Stereographic
  - Equidistant
  - Equisolid Angle
  - Orthographic
  - MK-6.5mm F2.0
- Support stereoscopic SBS/OU videos and photos
- Support VR photos with extension .vr.jpg (e.g. photos taken with VR180 cameras or Cardboard Camera app)
- Support color correction
- Support Xbox Controller

## Supported video formats

This app uses Media Foundation for video playback.  
Supported video formats are based on the Media Foundation.  
The video formats supported by Media Foundation also depend on the video extensions installed.
- MPEG-2 Video Extension
- HEVC Video Extensions
- VP9 Video Extensions
- AV1 Video Extension (Beta)

## Supported photo formats

- JPEG

## Controller mapping

| Action                                                | Motion Controller                | Xbox Controller
| :---------------------------------------------------- | :------------------------------: | :----------------------------------------:
| Move Pointer                                          | Motion Controller Pose           | Gaze
| Select                                                | Trigger Press                    | A Press
| Turn                                                  | Thumbstick Tilt Left / Right     | Right Thumbstick Tilt Left / Right
| Recenter                                              | Thumbstick Press                 | Right Thumbstick Press
| Play / Pause                                          | Touchpad Center Press            | Left Thumbstick Press
| Skip Back / Forward                                   | Touchpad Left / Right Press      | Left Thumbstick Tilt Left / Right
| Skip to Previous File or Rewind                       | Touchpad Left Long Press         | Left Bumper Press
| Skip to Next File                                     | Touchpad Right Long Press        | Right Bumper Press
| Volume Up / Down                                      | TouchPad Up / Down Press         | Left Thumbstick Tilt Up / Down
| Screen Scaling (Rect mode only)                       | Thumbstick Tilt Up / Down        | Right Thumbstick Tilt Up / Down
| Zoom (180 Fisheye mode only)                          | Thumbstick Tilt Up / Down        | Right Thumbstick Tilt Up / Down
| Open Windows File Picker (Videos Library)             | Menu Long Press                  | Menu or Y Long Press
| Open Windows File Picker (Pictures Library)           | Trigger Press + Menu Long Press  | Right Trigger Press + Menu or Y Long Press
| Open Folder Picker                                    | Menu Long Press                  | Menu or Y Long Press
| Show / Hide App-specific File Picker                  | Menu Press                       | Menu or Y Press
| Move Previous / Next Page in App-specific File Picker | Touchpad Left / Right Long Press | Left / Right Bumper Press
| Show / Hide Player UI                                 | Grip Press                       | X Press
| Show / Hide Settings UI                               | Grip Long Press                  | B Press

## File type associations

| File formats            | File extensions        |
| :---------------------- | :--------------------- |
| JPEG                    | .jpg, .jpeg            |
| Audio Video Interleave  | .avi                   |
| Advanced Systems Format | .asf, .wmv             |
| MPEG-2 Program Stream   | .mpg                   |
| MPEG-2 Transport Stream | .ts, .mts, .m2t, .m2ts |
| QuickTime File Format   | .mov                   |
| MP4                     | .mp4, .m4v             |
| Matroska                | .mkv                   |
| WebM                    | .webm                  |
