![PD Soluções](./pds-logo-v2.svg)

# Generic Validator to AdonisJS

A abstract class that defines methods to you write to do a [Generic CRUD](https://github.com/pdsolucoes/generic-crud-controller-adonis5):

* create

    Method to create a new entity.

* updateById
    
    Method to update an entity by ID.

* findById

    Method to find an entity by ID, by default receives an object with _id_ key as number. You can overwrite.

* getPaginate

    Method to return many paged entities. It receives the following object:

    ```typescript
    {
        page: number
        limit: number
        filter: string
    }
    ```
    If there was _page_ key, the _limit_ key must also exist. All elements are optional. You can overwrite.