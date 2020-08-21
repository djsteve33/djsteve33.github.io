---
layout: post
title:      "To ERB or Not To ERB"
date:       2020-08-21 23:08:08 +0000
permalink:  to_erb_or_not_to_erb
---


I was recently introduced to ERB and I thought I would write about it. ERB is a templating engine used in Sinatra. What is Sinatra? Sinatra is a free and open source software web application library and domain-specific language written in Ruby.  It is named after musician Frank Sinatra. Sinatra is a Ruby gem. Sinatra is classy web development dressed in a DSL DSL is Domain Specific Language. It is a Task Oriented Language – using code to write a new semantic language of expression. It is dependent on the Rack web server interface. Rack is a low-level adapter for web applications. It listens for and responds to web requests.

Sinatra, along with other major web frameworks, provide some means of view templating, allowing the view to be constructed using a combination of HTML and Ruby code. This allows us to greatly reduce duplication of HTML as well as generate content that can change based on the available data. This is how Facebook can support 2 billion users –– they create one template for the profile page, which then gets filled out with distinct, individualized user data from their servers.

Now, back to ERB. As I mentioned, ERB is a templating language written in Ruby. ERB is short for Embedded Ruby. It tells Sinatra to render the template specified inside of views directory and send the rendered output as a response. With ERB, we use two different types of tags: the substitution tag (<%=) and the scripting tag (<%).

The substitution tag evaluates Ruby code and then displays the results into the view. It opens with <%= and closes with %>. Inside of these tags, you can write any valid Ruby code that you want.

Example of a Substitution tags: <%= "Hello + World!" %>. The strings are concatenated first and then rendered on the page as Hello World! Another example is <%= 10 + 10 %>. What do you think would be rendered on the page? If you guessed 20, you're right! In general, we use substitution tags when we want to display some evaluation on the page.

And, then we have scripting tags. Scripting tags open with <% and close with %>. They evaluate, but do not actually display, Ruby code. What do you think the output in the browser would be from the below code?

<% if 10 == 20 %>
  <p>10 equals 20.</p>
<% else %>
  <p>10 does not equal 20.</p>
<% end %>

Of course, the second <p> is what will display in the browser.

Credit to Wikipedia and Flatiron School as a source of information for this blog.

