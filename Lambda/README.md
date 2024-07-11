𝐀𝐖𝐒 𝐂𝐥𝐨𝐮𝐝 𝐂𝐨𝐬𝐭 𝐎𝐩𝐭𝐢𝐦𝐢𝐳𝐚𝐭𝐢𝐨𝐧: 𝐈𝐝𝐞𝐧𝐭𝐢𝐟𝐲𝐢𝐧𝐠 𝐒𝐭𝐚𝐥𝐞 𝐑𝐞𝐬𝐨𝐮𝐫𝐜𝐞𝐬 𝐏𝐫𝐨𝐣𝐞𝐜𝐭 𝐔𝐬𝐢𝐧𝐠 𝐋𝐚𝐦𝐛𝐝𝐚

𝐏𝐫𝐨𝐣𝐞𝐜𝐭 𝐎𝐯𝐞𝐫𝐯𝐢𝐞𝐰:

This project aims to optimize AWS costs by identifying and deleting stale EBS snapshots using AWS Lambda. Users often create EC2 instances with associated volumes and take snapshots regularly. However, when EC2 instances and volumes are deleted, snapshots are sometimes forgotten, leading to unnecessary costs. This project will automate the process of fetching, filtering, and deleting stale snapshots.

𝐈𝐦𝐩𝐥𝐞𝐦𝐞𝐧𝐭𝐚𝐭𝐢𝐨𝐧 𝐄𝐱𝐚𝐦𝐩𝐥𝐞:

In this project, we'll create a Lambda function that identifies EBS snapshots that are no longer associated with any active EC2 instances and deletes them to save on storage costs.

𝐏𝐫𝐨𝐣𝐞𝐜𝐭 𝐒𝐭𝐞𝐩𝐬:

𝟏.𝐅𝐞𝐭𝐜𝐡 𝐀𝐥𝐥 𝐄𝐁𝐒 𝐒𝐧𝐚𝐩𝐬𝐡𝐨𝐭𝐬:
   - Use AWS Lambda to retrieve a list of all EBS snapshots in the AWS account.

𝟐.𝐅𝐢𝐥𝐭𝐞𝐫 𝐎𝐮𝐭 𝐒𝐭𝐚𝐥𝐞 𝐒𝐧𝐚𝐩𝐬𝐡𝐨𝐭𝐬:
   - Identify snapshots that are no longer associated with any active EC2 instances or volumes (stale snapshots).

𝟑.𝐃𝐞𝐥𝐞𝐭𝐞 𝐒𝐭𝐚𝐥𝐞 𝐒𝐧𝐚𝐩𝐬𝐡𝐨𝐭𝐬:
   - Safely delete the identified stale snapshots to optimize storage costs using AWS Lambda.

𝐍𝐨𝐭𝐞:
- If you have purposefully created snapshots, you can protect them using conditional statements based on their age, such as keeping snapshots that are 3 months old, 6 months old, etc.
