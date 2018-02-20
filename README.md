# Activemodel Relationships

## Specification

To produce an app in rails that does the following:

* Has a one to many link between two resources
* Contains full CRUD functionality
* The resources are associated with each other within a view
* Contains proper dependencies between the data: when a records dependency is deleted, that record is also deleted

## Implementation

* The two resources were authors, and books, where one author can have many books.
* Using both controllers, the CRUD methods were implemented for both resources.
* You can either view the data by listing the books and their authors beside each, or by listing all authors, and the books they have written, depending on which view file is used.
* Achieved by implementing the following line in the Author model
`has_many :books, dependent: :destroy`
