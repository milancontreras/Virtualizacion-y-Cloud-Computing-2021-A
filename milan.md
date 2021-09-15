# Tutorial: Automatically trigger MediaConvert jobs on S3 objects and get notifications when the jobs finish

A watchfolder is a common method for automating video ingest and delivery workflows.  Users with video ready for delivery upload their files to a known storage location.  The upload automatically triggers an ingest workflow that converts the video to formats suitable for delivery and stores them in the cloud for on-demand viewing.   The Serverless Video Conversion Watchfolder Workflow solves this problem by using [Amazon S3](https://aws.amazon.com/s3), [AWS Lambda](https://aws.amazon.com/lambda/), [AWS MediaConvert](https://aws.amazon.com/mediaconvert/), [Amazon CloudWatch Events](https://aws.amazon.com/cloudwatch) and [Amazon Simple Notification Service](https://aws.amazon.com/sns).

The workflow will create the following outputs for each video uploaded to the WatchFolder S3 bucket /inputs folder:
- An Apple HLS adaptive bitrate stream for playout on multiple sized devices and varying bandwiths.
- An MP4 stream
- Thumbnail images collected at intervals
