# Expo Camera Image Distortion Bug

This repository demonstrates a bug in Expo's Camera API where setting a custom resolution leads to image distortion. The preview displays correctly, but the captured image is of the wrong size or distorted.  The solution involves carefully managing the aspect ratio to ensure consistent image dimensions.

## Bug Report

When using `Camera.takePictureAsync` with a custom resolution, the captured image is distorted or has unexpected dimensions despite the preview appearing correctly.  This issue is likely caused by a mismatch between the aspect ratio of the preview and the captured image. The problem is isolated to custom resolutions; default resolutions seem to work properly.