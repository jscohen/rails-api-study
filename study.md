# Rails as an API Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   We'll use our [Rails API Template](https://github.com/ga-wdi-boston/rails-api-template)
    repository as the basis for our rails applications.
    This template excludes the "view" layer.

## Required Readings

-   Better Explained
    -   [Starting Ruby on Rails: What I Wish I Knew](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
        (sections 3 and 4)
    -   [Intermediate Rails: Understanding Models, Views and Controllers](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
        (up to and including "Quick Controllers")
-   Ruby on Rails Guides
    -   [Rails Routing from the Outside](http://guides.rubyonrails.org/routing.html)
        (up to and including chapter 2.6)
    -   [Action Controller Overview](http://guides.rubyonrails.org/action_controller_overview.html)
        (up to and including chapter 4.5)
    -   [The Rails Command Line](http://guides.rubyonrails.org/command_line.html)
        (up to and including chapter 1.4)

## Additional Resources

-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)

## Define Model Responsibilities

In your own words, define what the responsibilities of the model layer are in
Rails.

```md
The model layer in Rails talks to the database and has classes to receive db data, which flows to the rest of the app.  In addition, the model performs most of the business logic.
```

## Define Controller Responsibilities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
The controller layer handles client requests such as data submissions and sessions work.  It is really the server layer of the application.
```

## Define Router Responsibilities

In your own words, define what the router does in Rails.

```md
The router handles HTTP requests and creates paths based on each one to the resource.  It also transfers the correct web page to the view.
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
When you input an HTTP request such as GET to a url, the router matches it to a controller action.  So if you request a specific page, the router finds that resource and dispatches to the controller with the ID of the page and the GET request.  The controller is the server layer, so it sends the logic and markup and styles of the page to the view layer so the client can see.
```
