## Amazon Elastic Transcoder
Convert media files from S3 into required format.

**Jobs**: Can convert upto 30 different formats in one job.
**Pipeline**: Jobs can be added to pipeline and are executed in FIFO. If resources are available, the jobs are processed in parallel. Hence the jobs thats added later might have completed before the one in front of queue. Jobs that don't have enough resource will wait.
**Presets**: Templates for format conversions that can be used in jobs. Default templates like iPhone and iPad are available.
**Notifications**: SNS notifications can be sent if job starts, completes or errors out.
## Amazon Kinesis Video Streams
Fully managed service which lets to stream videos to the cloud, build applications for real-time video processing or batch processing.