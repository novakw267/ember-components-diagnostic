# Ember Components Diagnostic

Record your responses inside the fenced code blocks below each question.

1.  Give an example of a visual hierarchy that could be modeled with components. Explain why each piece might be it's own component.

    ```md
    <!-- Maybe a menu for an online ordering site. You could have a list of types of food as then branching out from each of those would be the actual items in those types. So it would be restaurant has many types of food which each have many types of recipies.  -->
    ```
    <!-- I am wonder if you were looking for an actual picture of a relationship tree, or if you just wanted me to break it down like so. Also did you want actual examples of how you would structure it in ember? -->

1.  What is the command to generate a new component called '`my-map`'?

    ```sh
    # ember generate component my-map
    ```

1.  What files are created and/or edited to produce a component, and what are their responsibilities?

    ```md
    <!-- an <component-name>.hbs index.hbs <component-name>.js and the router-->
    ```

1.  Suppose you have a component '`my-contact`', which is loaded from
    '`app/contacts/template.hbs`' when visiting the `/contacts` route. What is
    the syntax (code that is written) to render this component inside that template?

    ```html
    <!-- {{#each model as |my-contact|}} -->
    ```

1.  Each contact has multiple phone numbers. Suppose you also have '`my-phone`'
    nested under '`my-contact`'. What is the code you would write in
    '`app/components/my-contact/template.hbs`' to load the nested component and
    pass it data?

    ```html
    <!-- {{#each model as |my-contact|}}
  {{my-contact/my-phone
     list=list
   }} -->
    ```
      <!-- I found these two questions weirdly worded based on the file structure. I was confused if it wasn't supposed to be app/templates/contacts based on yesterdays lesson. So I was confused on which part of the generated files we were supposed to be referencing as an example.  -->
