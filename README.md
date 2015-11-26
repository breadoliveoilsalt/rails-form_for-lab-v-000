# `form_for` Lab

## Objectives

1. Use `form_for` to build a `new` form
2. Use `form_for` to build an `edit` form
3. Mass assign form data to `ActiveRecord` instances on `new` and `edit`
4. Build RESTFul actions for `new`, `create`, `edit`, and `update`, with the correct routes and route helper urls.


## Instructions

For this lab you will be implementing all of the functionality from scratch, including building out the models, views, and controllers for the `SchoolClass` and `Student` resources.

Below is what will be needed for each component of the MVC structure:

* **Models** - Create a `SchoolClass` model, along its associated database table. The `SchoolClass` table should have the columns: `title:string` and `room_number:integer`. The `Student` model and database table have already been created for you.

* **Controllers** - Create controller files for `school_classes` and `students`. Build out the `new`, `create`, `show`, `edit`, and `update` actions in each of the controllers.

* **Views** - Create a show page for each resource, along with `new` and `edit` forms.

You will also need to create routes for each path mentioned above.

The tests for this application are located in the `spec/controllers/`, `spec/features/`, and `spec/models/` directories.


## Requirements

Utilize the `form_for` methods for all four of the forms and integrate each `form_for` call with the respective controller actions. Also make sure to utilize the `<%= f.submit %>` submit button syntax to have the button text automatically generated.

Since you're using `form_for`, make sure you are using strong parameters for the controller `create` and `update` actions, if you don't remember how to do it, here is how we implemented strong params in the README: `@post.update(params.require(:post).permit(:title, :description))`. (hint: you can pass the strong parameter call to the `new` method just like we did on `update`)

If you run into issues drawing the routes, inspect element on the forms to see what path `form_for` is automatically trying to pass the form data to.


## Resources

* [Reading](https://github.com/learn-co-curriculum/rails-form_for-on-edit-readme)

* [Documentation](http://api.rubyonrails.org/classes/ActionView/Helpers/FormHelper.html)