# IAM
## Create policy
#### Service:

*CodeCommit*

#### Actions:

*All CodeCommit actions*

Access level:
- List.
- Read.
- Write.

#### Resources:

*All resources*

## Review policy
#### Name:

*<user>-git*

#### Description:

*Grant all privileges to user-devs.*

## Add user to group
#### Create group:

**Group name:** <user>-git

#### Policy

*<user>-git*

## Add user
#### User name:

*<user>-devs*

#### Add user to a group:

Programmatic access checkbox **ON**.

## Add user to a group

*<user>-git*