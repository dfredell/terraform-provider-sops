# Changes

## v1.2.1

- Fixed a bug where UniformBucketLevelAccess and BucketPolicyOnly were not
  being sent in all cases.

## v1.2.0

- Add support for UniformBucketLevelAccess. This configures access checks
  to use only bucket-level IAM policies.
  See: https://godoc.org/cloud.google.com/go/storage#UniformBucketLevelAccess.
- Fix userAgent to use correct version.

## v1.1.2

- Fix memory leak in BucketIterator and ObjectIterator.

## v1.1.1

- Send BucketPolicyOnly even when it's disabled.

## v1.1.0

- Performance improvements for ObjectIterator and BucketIterator.
- Fix Bucket.ObjectIterator size calculation checks.
- Added HMACKeyOptions to all the methods which allows for options such as
  UserProject to be set per invocation and optionally be used.

## v1.0.0

This is the first tag to carve out storage as its own module. See:
https://github.com/golang/go/wiki/Modules#is-it-possible-to-add-a-module-to-a-multi-module-repository.