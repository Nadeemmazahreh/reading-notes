## Django Forms   
    An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server. The Form class is the heart of Django's form handling system. It specifies the fields in the form, their layout, display widgets, labels, initial values, valid values, and (once validated) the error messages associated with invalid fields. The declaration syntax for a Form is very similar to that for declaring a Model, and shares the same field types (and some similar parameters). This makes sense because in both cases we need to ensure that each field handles the right types of data, is constrained to valid data, and has a description for display/documentation.


## Form Fields 
    BooleanField, CharField, ChoiceField, TypedChoiceField, DateField, DateTimeField, DecimalField, DurationField, EmailField, FileField, FilePathField, FloatField, ImageField, IntegerField, GenericIPAddressField, MultipleChoiceField, TypedMultipleChoiceField, NullBooleanField, RegexField, SlugField, TimeField, URLField, UUIDField, ComboField, MultiValueField, SplitDateTimeField, ModelMultipleChoiceField, ModelChoiceField.

## Form Arguments 
    -   required: If True, the field may not be left blank or given a None value. Fields are required by default, so you would set required=False to allow blank values in the form.
    -   label: The label to use when rendering the field in HTML. If a label is not specified, Django will create one from the field name by capitalizing the first letter and replacing underscores with spaces (e.g. Renewal date).
    -   label_suffix: By default, a colon is displayed after the label (e.g. Renewal date:). This argument allows you to specify a different suffix containing other character(s).
    -   initial: The initial value for the field when the form is displayed.
    -   widget: The display widget to use.
    help_text (as seen in the example above): Additional text that can be displayed in forms to explain how to use the field.
    -   error_messages: A list of error messages for the field. You can override these with your own messages if needed.
    -   validators: A list of functions that will be called on the field when it is validated.
    -   localize: Enables the localization of form data input (see link for more information).
    -   disabled: The field is displayed but its value cannot be edited if this is True. The default is False.

## Forms URL configurations 
    ```
    urlpatterns += [
    path('book/<uuid:pk>/renew/', views.renew_book_librarian, name='renew-book-librarian'),]
    ```


## Forms Template
    ```
    {% extends "base_generic.html" %}

    {% block content %}
    <h1>Renew: {{ book_instance.book.title }}</h1>
    <p>Borrower: {{ book_instance.borrower }}</p>
    <p{% if book_instance.is_overdue %} class="text-danger"{% endif %}>Due date: {{ book_instance.due_back }}</p>

    <form action="" method="post">
        {% csrf_token %}
        <table>
        {{ form.as_table }}
        </table>
        <input type="submit" value="Submit">
    </form>
    {% endblock %}
    ```

