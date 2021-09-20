# Changelog

All notable changes to this project will be documented in this file.

**NOTE:** Breaking changes may occur prior to the 1.0.0 release. Please update with caution.

## 0.9.6 (2021-09-10)

### Improvements and new features:

- Added case-ignoring when searching.
- Old parameters of read and write stages are cleaning now after the source type change.
- Added check of resource limits on pipeline start.
- "Run" button is now disabled, when changes of pipelines/jobs are not saved.

### Fixed:

- Fixed error 401 when pushing some buttons after long inactivity.
- Fixed Zoom and Pan Tool icon that save the previous value from the recently opened job/pipeline.
- Fixed text offset in Pipelines/Jobs lists, when changing the size of the browser window.

## 0.9.5 (2021-08-27)

### Improvements and new features:

- Added check during import that job/pipeline parameters exist in project params.
- Added custom SQL option to Read stage.
- Added IAM support for IBM COS storage.

### Fixed:

- Fixed white screen issue on the Job List page after switching to another project.

## 0.9.4 (2021-07-30)

### Improvements and new features:

- Added a public buckets support of AWS S3 due to the separation of AWS S3 and IBM COS in the Configuration panel.
- Jobs or pipelines export/import are available via JSON instead of string.
- On the Pipelines screen Search field doesn't clear after running pipeline.

### Fixed:

- Fixed the Run button after stopping pipeline in the Pipeline Designer.
- Fixed displaying Jobs and Pipelines lists after sorting or running.
- Fixed status "Terminated" in the Pipeline Designer.
- Fixed the displaying of an orange warning header about saving.

## 0.9.3 (2021-07-16)

### Improvements and new features:

- Added a warning header about saving in Designer mode.
- Added ability to rerun pipeline after error.
- New pipeline status "Terminated".
- The "Stop" button now terminates pipeline.
- The pipeline cron icon is hidden for now.
- Log button is avalilable in Job Designer when job status is Running.
- Spark can instantiate more than two executors.

### Fixed:

- Fixed Last Edit date in pipeline list for firefox.
- Fixed resume/stop functions for pipelines.
- Fixed display of search results in pipeline list and job list.
- Fixed help text for Read and Write stages.
