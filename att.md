In terms of solution for multiple pages. We suggest two solutions:

### Create a custom upstream - Like as SPCS project implementation.
  - We create a custom upstream from FCL. https://pantheon.io/docs/create-custom-upstream/
  - We build some functions on theme setting and Admin can upload logo, background...
  - With each movie page, we will create a new site base on custom upstream.

  **Advantages:**
  - We can easy develop style for each site.
  - We update on custom upstream and apply for each site by the dashboard UI.
  - Easy to manage content for each site/movie.
  - If there is a problem, it will affect only one site.

  **Disadvantages:**
  - It's probably complex on single site on.
  - High price.
  - Developer must join for creating site new new site/movie.
  - If there is update on component, it has to apply update before using it on site.

### Create one site base on FCL.
  - Create a content type for main site:

    http://start.att.net/exclusive/audience

    http://start.att.net/exclusive/audience/originals

    http://start.att.net/exclusive/audience/documentaries

  - Create a content type for landing page movie. Example pages:

    http://start.att.net/exclusive/audience/condor

    http://start.att.net/exclusive/audience/alone-in-the-game-documentary ...

    > This content of this content type will manage the movie information. It will support editor upload background, logo and order menu.

  - Create a content type for subpage movie. For examples:

    http://start.att.net/exclusive/audience/condor

    http://start.att.net/exclusive/audience/condor/episodes ...

    > It will provide some options for displaying logo, menu...
    > It will have reference field to the landing page movie for loading background, logo... on subpage.

   - If customer want to setup domain for each movie, it already has solution for it.

  **Advantages:**
    - Maintain on only one site.
    - Editor can create site/movie page themeselves.
    - Easily reuse component.
    - Manange(content, user) on one place.
    - Cheaper price than option 1.

  **Disadvantages:**
    - Quite complex on content permission, for example: If client want to assign each editor for each movie.
    - If there is a problem, it will affect all sites/movies.
