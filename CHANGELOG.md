# Change Log

All notable changes to this project will be documented in this file.

<a name="unreleased"></a>
## [Unreleased]



<a name="v1.12.0"></a>
## [v1.12.0] - 2020-06-16

- fix: Fixed patterns applying ([#30](https://github.com/terraform-aws-modules/terraform-aws-lambda/issues/30))
- fix: Fixed DUMP_ENV logging level ([#28](https://github.com/terraform-aws-modules/terraform-aws-lambda/issues/28))


<a name="v1.11.0"></a>
## [v1.11.0] - 2020-06-16

- fix: Fixed IAM policy attachment with multiple functions ([#26](https://github.com/terraform-aws-modules/terraform-aws-lambda/issues/26))


<a name="v1.10.0"></a>
## [v1.10.0] - 2020-06-14

- feat: Added support for variety of options for source_path, closes [#12](https://github.com/terraform-aws-modules/terraform-aws-lambda/issues/12) ([#25](https://github.com/terraform-aws-modules/terraform-aws-lambda/issues/25))
- Updated examples and readme
- Added more samples to examples/simple/main.tf
- package.py - Log directories with ending /
- package.py - Log skipped items + made uniform some messages
- package.py - Added support for comments in patterns
- package.py - Renamed: logger -> log
- feat: Added ZipContentFilter class to apply patterns filtering
- package.py - Fixed and improved logging
- package.py - Added BuildPlanManager initial implementation
- package.py - Fixed building in docker
- package.py - Implemented ZipFileStream.write_file
- feat: In-place zip archiving
- package.py - Removed dir changing on zip archive generation
- package.py - Simplified emit_dir_files func
- package.py - Fixed timestamp appling
- package.py - Added hidden hash command to calculate Lambda's content hash
- package.py - Finished ZipFileStream.write_dirs implementation
- package.py - Moved borrowed ZipInfo.from_file to a ZipWriteStream class
- package.py - Added initial ZipFileStream skel
- package.py - Move out inner functions from *_command functions
- feat: Added pid to the prepare stage log records


<a name="v1.9.0"></a>
## [v1.9.0] - 2020-06-12

- feat: Added AWS CodeDeploy group name to outputs


<a name="v1.8.0"></a>
## [v1.8.0] - 2020-06-12

- fix: Create AWS CodeDeploy resources conditionally
- fix: Do not create AWS Cloudwatch log group for Lambda Layers


<a name="v1.7.0"></a>
## [v1.7.0] - 2020-06-12

- feat: Add Cloudwatch Logs resources (or use existing) ([#24](https://github.com/terraform-aws-modules/terraform-aws-lambda/issues/24))


<a name="v1.6.0"></a>
## [v1.6.0] - 2020-06-11

- feat: Added package debug levels


<a name="v1.5.0"></a>
## [v1.5.0] - 2020-06-10

- fix: Added dependency for aws_s3_bucket_object, fixes [#15](https://github.com/terraform-aws-modules/terraform-aws-lambda/issues/15) ([#19](https://github.com/terraform-aws-modules/terraform-aws-lambda/issues/19))
- feat: Added support for one-shot artifacts build to skip recreation of missing packages ([#20](https://github.com/terraform-aws-modules/terraform-aws-lambda/issues/20))


<a name="v1.4.0"></a>
## [v1.4.0] - 2020-06-10

- feat: Added deploy module to do complex deployments using AWS CodeDeploy ([#17](https://github.com/terraform-aws-modules/terraform-aws-lambda/issues/17))
- feat: Stable zip archives - v1 ([#18](https://github.com/terraform-aws-modules/terraform-aws-lambda/issues/18))
- feat: Added better support for Lambda Alias resources via separate submodule ([#14](https://github.com/terraform-aws-modules/terraform-aws-lambda/issues/14))
- feat: Reliable passing build plan by a separate file + minor changes ([#13](https://github.com/terraform-aws-modules/terraform-aws-lambda/issues/13))


<a name="v1.3.0"></a>
## [v1.3.0] - 2020-06-07

- fix: Computed values in number of policies


<a name="v1.2.0"></a>
## [v1.2.0] - 2020-06-07

- feat: Added support for Lambda Permissions for allowed triggers ([#11](https://github.com/terraform-aws-modules/terraform-aws-lambda/issues/11))
- docs: Added link to apigateway-v2 module


<a name="v1.1.0"></a>
## [v1.1.0] - 2020-06-05

- feat: Added 4 new ways to customize IAM policies for Lambda Function ([#10](https://github.com/terraform-aws-modules/terraform-aws-lambda/issues/10))
- Fixed README
- Updated README formatting


<a name="v1.0.0"></a>
## [v1.0.0] - 2020-06-04

- Updated README formatting
- Initial terraform-aws-lambda implementation
- Added example of Dockerfile for custom AWS Lambda build env
- Added initial draft implementation of lambda.py and package.tf


<a name="v0.0.1"></a>
## v0.0.1 - 2020-06-02

- first commit


[Unreleased]: https://github.com/terraform-aws-modules/terraform-aws-lambda/compare/v1.12.0...HEAD
[v1.12.0]: https://github.com/terraform-aws-modules/terraform-aws-lambda/compare/v1.11.0...v1.12.0
[v1.11.0]: https://github.com/terraform-aws-modules/terraform-aws-lambda/compare/v1.10.0...v1.11.0
[v1.10.0]: https://github.com/terraform-aws-modules/terraform-aws-lambda/compare/v1.9.0...v1.10.0
[v1.9.0]: https://github.com/terraform-aws-modules/terraform-aws-lambda/compare/v1.8.0...v1.9.0
[v1.8.0]: https://github.com/terraform-aws-modules/terraform-aws-lambda/compare/v1.7.0...v1.8.0
[v1.7.0]: https://github.com/terraform-aws-modules/terraform-aws-lambda/compare/v1.6.0...v1.7.0
[v1.6.0]: https://github.com/terraform-aws-modules/terraform-aws-lambda/compare/v1.5.0...v1.6.0
[v1.5.0]: https://github.com/terraform-aws-modules/terraform-aws-lambda/compare/v1.4.0...v1.5.0
[v1.4.0]: https://github.com/terraform-aws-modules/terraform-aws-lambda/compare/v1.3.0...v1.4.0
[v1.3.0]: https://github.com/terraform-aws-modules/terraform-aws-lambda/compare/v1.2.0...v1.3.0
[v1.2.0]: https://github.com/terraform-aws-modules/terraform-aws-lambda/compare/v1.1.0...v1.2.0
[v1.1.0]: https://github.com/terraform-aws-modules/terraform-aws-lambda/compare/v1.0.0...v1.1.0
[v1.0.0]: https://github.com/terraform-aws-modules/terraform-aws-lambda/compare/v0.0.1...v1.0.0
