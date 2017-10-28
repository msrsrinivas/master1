# Approach:-

The best approach is to pulling the group members using a impersonating normal account that has access to the group. Create a dummy user (i.e. admin.dealsiq@pwc.com) using the service account, impersonate the dummy user. Using that user Id and Group id, fetch the group member information. 

Dummy user will have elevated permissions while compared to the normal user i.e. providing only group access permission to this user and it will not have highest privileges to touch the sensitive information of the group as like service account.

Dummy user creation and providing the required permissions need to be taken care by infra team.

