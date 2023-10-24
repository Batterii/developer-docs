# Understanding User Workspace Permissions in Vurvey.app

In Vurvey.app, we've implemented various permissions to ensure each user can perform tasks
that align with their role. Here's an overview of how the permissions work:

## 1. Confirmed Workspace Members

If you're a confirmed member of a workspace, you can:

- **Read**: View the contents of the workspace.
- **Create, Read, Update, Delete**: Perform these operations on various elements such as
  Attribute Categories, Segments, DynamicSegments, ContactTags, etc.
  - For example, you can create a new 'Attribute Category' or update an existing
    'Segment'.
- **Add, Remove**: Add or remove items such as 'Contacts'.
  - For example, you might add a new contact to your workspace or remove an existing one.
- **Apply, Remove**: Apply or remove tags on 'ContactTag'.
  - For example, you might tag a contact as 'VIP' or remove the 'VIP' tag.

## 2. Confirmed Workspace Administrators and Owners

If you're a confirmed workspace administrator or owner, you have all the permissions of a
confirmed member, plus:

- **Update**: Make changes to the workspace itself.
- **TremendousSettings**: Adjust the specific settings related to 'Tremendous' in your
  workspace.
- **AddManager, AddAdministrator, MakeManager, MakeAdministrator, Remove**: Perform these
  operations on 'Member'.
  - For example, you can promote a member to the role of an administrator or demote an
    administrator to a member.

## 3. Confirmed Workspace Owners

If you're a confirmed owner of a workspace, you have all the permissions of an
administrator, plus:

- **ManageBilling**: Control the billing details for the workspace.
- **Delete**: Delete the workspace.
- **Cancel**: Cancel the workspace.
- **AddOwner, MakeOwner**: Make a member or administrator an owner.

# Understanding Survey Permissions in Vurvey.app

Surveys are a key part of Vurvey.app, facilitating data collection and feedback.
Understanding when and how users can read and respond to surveys is crucial for maximizing
the platform's utility.

## Ability to View a Survey: Viewing it in the Workspace site (This is different than "Responding to a Survey"...See Creating Reesponses for a Survey for this)

The ability to "view" a survey means a user can view the survey's content. This includes
the survey's questions, structure, and potentially earlier responses and other meta-data
such as who created the survey, the survey's current status, etc.

### Permissions for Reading a Survey

- **Confirmed Workspace Members**: Confirmed members of a workspace have the permission to
  read any survey within that workspace. This means they can view the content, structure,
  and other details of a survey. However, they cannot modify the survey unless they have
  been given additional permissions.

- **User Whom Created the Survey**: The user in a workspace that created the survey can
  always view the survey. They can view all the details, follow the responses, and make
  adjustments if necessary.

- **Workspace Administrators and Owners**: Individuals with administrative or ownership
  roles in a workspace can read all surveys within that workspace.

### Examples

1. **Workspace Members**: If you're a member of a marketing team workspace, you can read a
   survey created in that workspace to understand the customer feedback being collected.
2. **User Whom Created the Survey**: As the creator of a survey on user experience, you
   can read the survey to ensure the questions are formulated correctly and to follow the
   incoming responses.
3. **Workspace Administrators and Owners**: As an owner of a workspace, you can read a
   survey created by your team member to understand its structure and purpose better.

## Creating Responses for a Survey (aka, taking the Survey)

Creating responses for a survey means a user can answer the survey questions and submit
their responses.

### Permissions for Creating Responses

- **Survey Responders**: The precise group of users who can respond to a survey can vary
  depending on the survey's access level and if the survey is in Draft, Open (live), Closed.
  Additionally, surveys can be configured to allow users to respond only once, or as many times as they wish.

  Examples:
  1. If the Survey is published (live) and it is public, then anyone can view the preview link or take the survey provided they have the link.
  2. If it is in Draft mode and it is Public, then you need to login and be a member of the workspace of the survey to be able to view the survey preview.
  3. If the Survey is Private and Open, then you have to be invited to view and take the Survey or be a member of the workspace to view the preview.
  4. If the Survey is Closed, no one can take the survey. Workspace members can still view the survey and responses and analytics from within the workspace.

Remember, the ability to read a survey and the ability to respond to a survey are
distinct. A user might be able to read a survey without being able to respond to it, or
vice versa, depending on the permissions and the distribution of the survey.
