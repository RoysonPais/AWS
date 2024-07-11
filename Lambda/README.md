AWS Cloud Cost Optimization: Identifying Stale Resources Project Using Lambda

Project Overview:

This project aims to optimize AWS costs by identifying and deleting stale EBS snapshots using AWS Lambda. Users often create EC2 instances with associated volumes and take snapshots regularly. However, when EC2 instances and volumes are deleted, snapshots are sometimes forgotten, leading to unnecessary costs. This project will automate the process of fetching, filtering, and deleting stale snapshots.

Implementation Example:

In this project, we'll create a Lambda function that identifies EBS snapshots that are no longer associated with any active EC2 instances and deletes them to save on storage costs.

Project Steps:

1.Fetch All EBS Snapshots:
   - Use AWS Lambda to retrieve a list of all EBS snapshots in the AWS account.

2.Filter Out Stale Snapshots:
   - Identify snapshots that are no longer associated with any active EC2 instances or volumes (stale snapshots).

3.Delete Stale Snapshots:
   - Safely delete the identified stale snapshots to optimize storage costs using AWS Lambda.

Note:
- If you have purposefully created snapshots, you can protect them using conditional statements based on their age, such as keeping snapshots that are 3 months old, 6 months old, etc.
