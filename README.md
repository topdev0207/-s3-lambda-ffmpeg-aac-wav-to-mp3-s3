
# S3 Bucket -> Lambda (FFMPEG Convert AAC,WAV to MP3) -> S3 Bucket

## Description

This is a serverless component that takes uploaded AAC, WAV audio files from one S3 Bucket, then using FFMPEG Lambda Layer converts them to MP3 and uploads to another S3 Bucket. It contains:

- an Input S3 Bucket that accepts WAV,AAC audio files.

- a Lambda that takes the WAV/AAC audio file from the Input S3 bucket, converts it to a MP3 one and uploads it to the Output bucket

- an Output S3 Bucket that receives MP3 files.

## Deployment Parameters

This component has one CloudFormation deployment parameter:

- `ConversionTimeout`, an optional parameter, represents the timeout of the Conversion Lambda function. By default it's 180 seconds.

## Latest Release - 1.0.0

- Initial release.

## Roadmap - Upcoming changes

Here are the upcoming changes that I'll add to this serverless component:

- ESLint
- Tests
