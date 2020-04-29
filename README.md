# Solo Capstone

Let's ship and present a product — solo! Combine some of the technologies that you've learned so far to build, launch, and pitch an interactive website.

## Contents <!-- omit in toc -->

- [Choosing A Project](#Choosing-A-Project)
- [Evaluation](#Evaluation)
- [Milestones + Rough Drafts](#Milestones--Rough-Drafts)
- [Technologies and Platforms](#Technologies-and-Platforms)
  - [CSS Frameworks](#CSS-Frameworks)
  - [jQuery](#jQuery)
  - [Back-End Libraries](#Back-End-Libraries)

## Choosing A Project

The project should meet three criteria:

1. You're interested in it
1. It can be deployed as an interactive website (i.e., not only HTML and CSS)
1. It is connected to the broader cultural moment

You don't have to use all the technologies below, but you need to decide early on whether the project will require a back-end or not.

For example, you could have a website that includes interactive charts, even if the underlying data is static. That would not require a back-end if you embedded the data into the HTML document itself.

Or you could use the built-in browser [fetch API][mdn-fetch] to pull in data from third-party datasources and APIs.

If you want visitors to enter data that persists between sessions / visible on multiple computers / etc. then you will need your own back-end to store that.

## Evaluation

You will be evaluated on your ability to organize your work, successfully ship a usable product, and present that project in a compelling way (via the presentation).

You can use any tools or technologies to achieve this so long as the final product is a live, on-the-web product people can use. If you save time by using powerful, off-the-shelf technologies, that should be reflected in more customer feedback, a more refined product, and a better presentation.

These are the questions we'll be using to evaluate your project:

1. Did you get consistent feedback on the the following throughout the project?
   - The design and overall experience of the site
   - The pitch / presentation
   - The structure of your database (if using a backend)
   - The structure of your HTML, CSS, and JavaScript
1. Did your project connect to the broader cultural moment / concerns?
1. Would a stranger in your project's intended audience be able to use your project without help from you?
1. Was your presentaiton clear, engaging, and paced well?

## Milestones + Rough Drafts

You will be working on the project and the presentation in parallel. Your aim is to get feedback early and often, which means you need to do more than just *describe* your plans.

Specifically...

- Before the first 10% of the project timeline, you should have:
  1. Pitched one or more ideas to your instructor and received feedback about which one makes the most sense
- Before the first 25%, you should have:
  1. Wireframes of all the screens you expect a user to interact with
  1. An outline of your presentation on Google Slides
- Before the first 50%, you should have:
  1. A live, on-the-web prototype of the product you can put in front of people and get real feedback (friends, family, classmates, etc.)
  1. A rough draft of the presentation
- Before the first 75%, you should have:
  1. A finalized version of the project with only a small number of bugs to fix
  1. A dry run of your final presentation

The goal isn't to eliminate surprises and plan out everything perfectly. There *will* be disruptive surprises. We need to work in a way that gives us breathing room to *handle* those surprises.

To achieve this, you will have to decide what is *absolutely essential* to the success of your final project and focus on those first.

## Technologies and Platforms

Below are the high-level technologies we've used over the course. Select some of them to use in your project.

- HTML
- CSS
- JavaScript (front-end / browser)
- JavaScript (back-end / Node)
- PostgreSQL
- Heroku

### CSS Frameworks

You should use a CSS framework for your project. Here are some ones we recommend:

- [Bootstrap][url-bootstrap]

  Bootstrap is the "kitchen sink" of CSS frameworks. It comes with many built-in, interactive components. This makes it easy to get quick, impressive results.

  The downside is that it can be challenging to change the look and feel. Bootstrap-based websites have a distinct "bootstrap-y" feel.

- [Bulma][url-bulma]

  Bulma is the opposite of bootstrap in many ways. It is less opinionated and provides fewer components out of the box. You can use it for the high-level structure (major sections, containers, alignment, etc.), but the finer-grained details are left up to you.

### jQuery

You will want to use [jQuery][url-jquery] to make it easier to interact with the page using JavaScript. Selecting and manipulating elements and event listening are much easier with jQuery.

### Back-End Libraries

- [Express][url-express]

  If you're buliding a database-backed JavaScript web application, you will be using Express.

  Use one of the previous Express-based projects as a starting point or use the [express generator][url-express-generator] to generate a "skeleton app".

  If you want to use Handlebars for your templates, run the following:

  ```console
  npx express cool-new-app --git --view hbs
  ```

  This will create a skeleton express application in the `cool-new-app` directory. Change `cool-new-app` to whatever you want.

- [Knex][url-knex]

  Knex is a Node library for generating generating and executing SQL queries. If you're using PostgreSQL, also install the `pg` library.

  Inside your project that means running:

  ```console
  npm install --save pg knex
  ```

  Look at previous projects to see how to set up `knex`. Run the following command to see what `knex` can do:

  ```console
  npx knex --help
  ```

  The documentation on the Knex website is thorough and consistent. You can also use this [Knex cheat sheet][url-knex-cheat-sheet].

- [Objection][url-objection]

  Objection is a library that uses Knex to interact with the database, but instead of interacting via SQL queries, we interact via JavaScript objects.

  If Objection is overwhelming or confusing, stick with Knex and plain SQL queries.

[url-bootstrap]: https://getbootstrap.com/docs/4.4/getting-started/introduction/
[url-bulma]: https://bulma.io/documentation/
[url-jquery]: https://jquery.com/
[url-express]: https://expressjs.com/
[url-express-generator]: https://expressjs.com/en/starter/generator.html
[url-knex]: http://knexjs.org/
[url-knex-cheat-sheet]: https://devhints.io/knex
[url-objection]: https://vincit.github.io/objection.js/
[mdn-fetch]: https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch
