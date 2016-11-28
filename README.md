# aws-lambda-automated-snapshots
Creates snapshots from volumes of EC2 instances that have the proper tags

This is based on the code from this blog post: https://serverlesscode.com/post/lambda-schedule-ebs-snapshot-backups/

# What's the difference?
I added the functionality to include the ec2 tags to the snapshot, downside is that now it makes a call to the API for each snapshot, it doesn't update them all at the same time (with just one call).
