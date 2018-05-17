In terms of solution for multiple pages. We suggest two solutions:

### 1. Create a custom upstream - Like as SPCS project implementation.
  - We create a custom upstream from FCL. https://pantheon.io/docs/create-custom-upstream/
  - We build some functions on theme setting where admin can upload logo, background...
  - For each movie page, we will create a new site base on custom upstream.

  **Advantages:**
  - We can develop easily style for each site.
  - If there is any change, we only need to update on upstream and it will show notification on dashboard UI about the update.
  - Easy to manage content for each site/movie.
  - If there is a problem, it will affect only one site.

  **Disadvantages:**
  - It's probably complex on single site on.
  - High price.
  - Developer must join for creating site new site/movie.

### 2. Create one site base on FCL.
  - Create a content type for main site:

    http://start.att.net/exclusive/audience

    http://start.att.net/exclusive/audience/originals

    http://start.att.net/exclusive/audience/documentaries

  - Create a content type for landing page movie. Example pages:

    http://start.att.net/exclusive/audience/condor

    http://start.att.net/exclusive/audience/alone-in-the-game-documentary ...

    > This content of this content type will manage the movie information. It will help editor to upload background, logo and to update order of menu item.

  - Create a content type for subpage movie. For examples: Cast information, episodes, talks.

    http://start.att.net/exclusive/audience/condor

    http://start.att.net/exclusive/audience/condor/episodes ...

    > It will provide some options for displaying logo, menu...
    > It will have reference field to the landing page movie for loading background, logo... on subpage.

  - If customer want to setup domain for each movie, we've already had solution for it.

  **Advantages:**
  - Maintain on only one site.
  - Editor can create site/movie page themeselves.
  - Easily reuse components.
  - Manange(contents, users) on one place.
  - Cheaper price than option [1](1-create-a-custom-upstream---like-as-spcs-project-implementation).

  **Disadvantages:**
  - Quite complex on content permission, for example: If client want to assign each editor for each movie.
  - If there is a problem, it will affect all sites/movies.
