# Role-based access control

RBAC  is an approach to restricting system access to authorized users. It is used by the majority of enterprises with more than 500 employees.

policy-neutral access-control mechanism defined around roles and privileges.

RBAC is a flexible access control technology whose flexibility allows it to implement Discretionary access control and Mandatory access control.

DAC is a type of access control defined by the Trusted Computer System Evaluation Criteria[1] "as a means of restricting access to objects based on the identity of subjects and/or groups to which they belong.

MAC is a type of access control by which the operating system or database constrains the ability of a subject or initiator to access or generally perform some sort of operation on an object or target.

User -->   Role --> Rights

there is some user want to use some folder or file in the company so to reach this file he must have some role example (if you are CO you can open this file) so this role it put for some people to access for some information in system.

1. in enterprise setting ==> access may be based on job function or role of a user.

2. payroll manager, project member ==> the developer, manager, owner and HR may have access for this file.

3. user then can activate one or more roles for themselves.


## Benefit

1. policy no need to update when a certain person with a role leaves the organization.

2. the new employees should be able to activate the desired role.

3.Revisiting least privilege : 

A- user can be in one role has access to a subset of the files.

![RBAC](https://github.com/naeemmusamh/Reading-note/blob/master/IMAGE/401/Role-based_access_control.jpg?raw=true)