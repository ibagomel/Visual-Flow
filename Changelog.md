# Changelog

All notable changes to this project will be documented in this file.

**NOTE:** Breaking changes may occur prior to the 1.0.0 release. Please update with caution.

## 0.9.17 (2022-03-18)

### Improvements and new features:

- New stage in the Job Designer - Sort.
- Improved the display of the Sort stage and its description.
- Created tooltips for the left menu on the Main screen.

### Fixed:

- All fields are disabled in Configuration panel when Job is running.
- In the Configuration panel, the sort type field is set to the default value.
- Fixed a stage color change after deleting of another saved stage in the Pipeline Designer.
- Fixed the display of the log icon when changing jobs in Job stage in the Pipeline Designer.
- Fixed the display of the outline/background of the Job stage in the Pipeline Designer.
## 0.9.16 (2022-03-04)

### Improvements and new features:

- Created and configured GitHub Actions self-hosted runner.
- Created general component to work with stage's tag.
- Added full query mode to Transformer stage.
- Validation project parameters in the pipeline.

### Fixed:

- Fixed display of White screen after double click on Container stage in 'Error' pipeline.
- Fixed incorrect stages coloring when interrupting the pipeline

## 0.9.15 (2022-02-18)wg

### Improvements and new features:

- New operations for DB2, Oracle, MySQL, PostgreSQL, MSSQL, Redshift(JDBC) - Truncate and Truncate Cascade.
- Created the clear button for fields with numbers. 
- Applied validation for project parameters, pipeline name.
- Added the star symbol to required fields in PD and JD.
- The ability to auto generate file name proposal during export.
- Added icon with tooltip on stages with missing/invalid parameters in the Pipeline Designer.
- The ability to go to the list of Jobs/Pipelines, when a user clicks on the appropriate square.

### Fixed:

- Fixed CDC error after click on confirm.
- Fixed warning after moving from the Overview page to the Jobs page and warning after deleting job/pipeline in console. 
- Confirm button is disabled, when there are empty required fields.

## 0.9.14 (2022-02-04)

### Improvements and new features:

- New parameter for STDOUT storage - Records quantity.
- Added ability to remove selected value from dropdown list in Pipeline and Job Designers. 
- The ability to add a stage by double-click.
- Updated and improved descriptions for:STDOUT storage, Remove duplicates and Transformer stages.
- Added a scrollbar for Info window.
- Improved error message when user enters more than 40 symbols in Job/Pipeline Name field.

### Fixed:

- Fixed incorrect display of the Orange header.
- Fixed an inscription above the arrows after editing.
- Fixed arrow colors when changing Output Paths value in the Job Stage.

## 0.9.13 (2022-01-21)

### Improvements and new features:

- New data storage - Redshift.
- Updated and improved description for: CDC, Union and Transformer stages, function Write mode.
- Adapted application logs to display user login information.
- Available action "Edit Child Node".

### Fixed:

- The arrow don't disappear, when changing storages for connecting.
- Fixed Read/Write stage validation on job level.
- Changed the order of links in the Join stage.
- Set the quantity of in-out arrows for each stage.
- Undo/Redo buttons are disabled in Job/Pipeline Designer before editing. 
- Fixed displaying of orange header.

## 0.9.12 (2021-12-24)

### Improvements and new features:

- New stage in Job Designer - Cache.
- Added Partition By SQL function to Write stage for IBM COS and AWS S3 storages.
- Adapted application logs to display user login information

### Fixed:

- Corrected Join stage description.
- Fixed custom SQL processing for PostgreSQL storage.

## 0.9.11 (2021-12-10)

### Improvements and new features:

- Added a full description for using the Transformer stage.
- New level in Logs window - Result.
- The search for the entered value does not depend on which register, it's displayed in Logs window.

### Fixed:

- Fixed Read and Write stages descriptions. 
- Container icon displays properly if Container stage was added to the created and launched pipeline. 
- Fixed displaying the orange header after editing.
- Adjusted malformed log configuration for Spark.
- Implemented 'Return all' function for Change data capture stage.  

## 0.9.10 (2021-11-12)

### Improvements and new features:

- New data source: Redis.
- The orange header with warning message is not displayed after clicking the Confirm button without changes.
- Logs filters are displayed as multiselect dropdown list.

### Fixed:

- Runtime information (logs, status) is cleared after saving the edited job.

## 0.9.9 (2021-10-29)

### Improvements and new features:

- New data sources: Cassandra, Mongo.
- Added time difference between current and UTC in Last run filter.
- Export files in a JSON format instead of Text.
- Added all statuses to Overview page.

### Fixed:

- Fixed data output in STDOUT storage.
- The Table field for MySQL/MSSQL/ORACLE/PostgreSQL storage stores a value set by the user in the Configuration panel.
- Removed the STDOUT storage from the list for Read stage. 
- Fixed editing the PARAMS panel of a new job, after running an existing one.
- Fixed editing a PALETTE/PARAMS panel, when the job was run and executed in Job Designer page.

## 0.9.8 (2021-10-15)

### Improvements and new features:

- Added tooltips for icons in Job and Pipeline designers.
- Filtered Logs are displayed after updating. 
- All statuses are available for sorting of jobs and pipelines in drop-down list.

### Fixed:

- Job logs URL contains both job ID and job Name.
- Fixed "white screen" displaying after the opening of Job/Pipeline Designer. If the pipeline or job was created via the API, then the appropriate message is shown.  
- Fixed the loading of a Job/Pipeline Designer after entering and saving params. 

## 0.9.7 (2021-10-02)

### Improvements and new features:

- New data sources: PostgreSQL, MySQL/Maria, MSSQL, Oracle.
- New pipeline stage for running custom code - Custom container.
- Added ability to specify resource units in Custom container configuration panel.
- Added logs button for Custom container stage.
- In job logs added total rows number for each job stage.
- The Stop button is displayed in "Pending" status.

### Fixed:

- Fixed the bug related to the display of a white screen after double click notification stage, when a pipeline is terminated.
- Fixed Info icon in Custom container configuration panel.
- Make "mount project params" is an optional field in the Custom container configuration.

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
