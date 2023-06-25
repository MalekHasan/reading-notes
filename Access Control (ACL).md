# Access Control (ACL)
## 5 steps to RBAC

1. What is Role Based Access Control (RBAC) and why do we care?  

***Role-Based Access Control (RBAC) is a security model that provides a structured approach for managing and controlling access to resources within a system or organization. In RBAC, access permissions are granted to users based on their assigned roles, rather than individually. Each role is associated with a set of permissions that define what actions or operations a user with that role can perform.***

2. Describe a Role/Permission heirarchy that you might implement using RBAC. 

***This RBAC hierarchy ensures that each user has the necessary permissions to fulfill their role without unnecessary access to sensitive information or functions. It follows the principle of least privilege, granting users the minimum permissions required to perform their job functions effectively while maintaining security.***

3. What approach might you take to implement RBAC?  

- ***Inventory your systems***
- ***Analyze your workforce and create roles***
- ***Assign people to roles***
- ***Never make one-off changes***
- ***Audit***

## wiki - RBAC

1. If Authentication is “you are who you say you are,” what is Authorization?

***Process of granting or denying access to specific resources or functionalities based on a user's authenticated identity and their permissions or privileges.***

2. Name three primary rules defined for RBAC.
- ***Role assignment: A subject can exercise a permission only if the subject has selected or been assigned a role.***

- ***Role authorization: A subject's active role must be authorized for the subject. With rule 1 above, this rule ensures that users can take on only roles for which they are authorized.***

- ***Permission authorization: A subject can exercise a permission only if the permission is authorized for the subject's active role. With rules 1 and 2, this rule ensures that users can exercise only permissions for which they are authorized.***

3. Describe RBAC to a non-technical friend.

***RBAC, or Role-Based Access Control, is a system where individuals are assigned specific roles within an organization. Each role has a set of permissions that determine what actions they can perform. It simplifies access management by granting permissions based on job responsibilities. RBAC enhances security by ensuring individuals only have access to what is necessary for their roles, reducing the risk of unauthorized access. It improves efficiency by streamlining access control and reduces the chances of errors or misuse of resources. RBAC provides clear accountability by linking actions to specific roles, making it easier to track and audit user activity.***

1. What Are access rights Associated with? The User? or The Role? Explain.

***Access rights are the ability to access resources and Access rights Associated with role. The access rights are the way to define your policy ,access control policy so we ask what is your role in the system and in the system what kind of resource can you access.***
2. Access Rights, or Authorization, is activated after a user successfully does what?

***Access rights or authorization are activated after a user successfully completes the process of authentication, which involves verifying their identity.***

3. Explain how RBAC might benefit a business.

***It's enhance the security because we take the permissions for each user in the system and each role in the system can access to a specific resources so we simplifies access management by centralizing permissions based on roles.***