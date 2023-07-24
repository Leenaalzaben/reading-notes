Question 1:

The key components of DRF permissions include:

1. Permission classes: These are the classes that define the rules for accessing API views or objects. They determine whether a request should be granted or denied based on factors such as authentication status, user roles, or custom conditions.

2. Global default permissions: You can specify a default permission class for all views in your API. This ensures that all views in your API are protected by a certain level of permission unless explicitly overridden.

3. View-level permissions: You can specify different permission classes for individual API views. This allows you to have fine-grained control over the access to each view based on specific requirements.

4. Object-level permissions: DRF also supports object-level permissions, which allow you to control access to individual objects within views. Object-level permissions are useful when you want to restrict access to specific objects based on additional conditions or ownership.

Question 2:

In SQL, the SELECT statement is used to retrieve data from a database. It allows you to specify which columns or expressions you want to retrieve from one or more tables, as well as any filtering or sorting criteria.

Question 3:

DRF (Django REST Framework) provides a set of powerful tools for building RESTful APIs in Django. One of its key features is the provision of generic views, which are pre-implemented views that encapsulate common behavior and simplify the API development process. These views are often referred to as DRF Generic Views.

DRF Generic Views offer a higher level of abstraction and reduce the amount of code you need to write to handle common tasks such as retrieving, creating, updating, or deleting model instances. They provide a standardized way to handle HTTP methods like GET, POST, PUT, PATCH, and DELETE for different use cases.
