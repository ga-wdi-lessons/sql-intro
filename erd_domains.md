# Domain Modeling & ERDs

## Learning Objectives

- Draw an Entity Relationship Diagram (ERD)
- Identify and diagram one-to-one, one-to-many and many-to-many relationships between data entities
- Distinguish between entities and attributes
- Discuss data normalization needs and techniques

## Framing

Developers employ **user stories** clarify the features we need for a good user experience. What is a user story?

> User stories are short, simple descriptions of a feature told from the perspective of the person who desires the new capability, usually a user or customer of the system. They typically follow a simple template:
>
> As a `type of user`, I want `some goal` so that `some reason`.
>
> Source: [Mountain Goat Software](https://www.mountaingoatsoftware.com/agile/user-stories)

We use them to prioritize order and scope. Today, we will identify the information required to support those user stories. We refer to this as the **Domain** or **Domain Model**. The Domain Model specifies the data and the relationships between this data. We use it to decide what needs to be persisted.

## Domain Modeling (20 minutes / 0:20)

Domain Modeling allows us to outline the data values that we need to persist.
- We only consider the attributes of our data, not the behavior of our application
- A domain model in problem solving and software engineering is a conceptual
model of all items and topics related to a specific problem
- It describes the various entities, their attributes, roles and relationships,
plus the constraints that govern the problem domain

The big takeaway here is that domain modeling **does not describe solutions to the problem**. Instead, it defines how our data is structured.

### ERDs

An ERD -- or **Entity Relationship Diagram** -- is a tool we use to visualize and describe the data relating to the major entities that will exist in our programs.
- Ultimately lends itself to planning out and creating our database table structure
- It allows us to outline the data in our application, not the behavior

### Example: An Orchard

Take a minute to look through the below diagram. Note down any observations you have.

![orchard example](images/orchard.png)

- The squares represent our entities and are filled with the attributes associated with our entity.
- The arrows between the squares indicate how the entities relate to one another.

### Relationships

![relationships](images/sample-relationships.png)

**One-to-one:** A Country has one Capital City
- Usually denotes that one entity should be an attribute of the other
- Usually separated for physical space considerations

**One-to-many:** A Location has many Cohorts
- The most common relationship you will define in WDI.

**Many-to-many:** A Membership has many Assignments through Submissions, and an Assignment has many Memberships through Submissions.
- Requires a join table. In this example, that is Submissions.

### Example: Garnet

![garnet_erd](images/Garnet_ERD.png)

ERDs get more complex the larger your application becomes. Nevertheless, they are still a useful tool when planning and developing. The instructors reference this diagram all the time!

### You Do: Library ERD (15 minutes / 0:35)

> 10 minutes exercise. 5 minutes review.

Come up with an example ERD for an application that manages a library.

#### You Do: ERD's for Web Pages in the Wild (15 minutes / 0:45)

> 10 minutes. 5 minutes review.

Now do the same thing, this time for a real world application. Make an ERD for the option that matches your group number below...

1. Amazon
2. Facebook
3. Reddit
4. ESPN
5. Twitter

## Break (10 minutes / 0:55)
