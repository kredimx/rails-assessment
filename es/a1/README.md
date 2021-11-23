# Part II
### El desafío del acortador de URL's

Tu misión será crear una REST API que sirva para crear links cortos, estos son más fáciles de compartir vía sms o por mensajes, a la par que permiten crear analytics sobre el consumo de dicho servicio.

Crea un repositorio para tu proyecto, puedes usar Github, Gitlab, Bitbucket, etc.

Cuando termines por favor compartenos tu repositorio y de ser posible los links de tu aplicación si lograste desplegarla.

+puntos extra si usas docker.



### CORE REQUIREMENTS
- As a visitor, I want to create an account for the app, so that I become an active user.
    Acceptance Criteria:
      - Application needs my name, email, and password.
      - Duplicated emails are not allowed.
      - Validates email input.
- As an active user I must be able to put a URL into the home page and get back a URL of the shortest possible length.

      AC:
        - You shouldn't use any gem or library that provides the short url algorithm
        - Inputting a valid URL should result in displaying the new shortened URL to the user.
        - Inputting an invalid URL should result in displaying errors to the user.

- As an active user I must be able to manage my links, edit, create, destroy, etc.

- Every time one short link is opened, the app must record visitors' data, such as `IP address`, `user agent`, `OS (if possible)`, `date`.

- Our app must differentiate between unique visitors (IP's) and recurrent visitors.

- As an active user, every time I share this link, I must be redirected to the full URL when we enter the short URL (ex: [http://app.com/aSdF](http://app.com/aSdF)​ =>​ [​https://google.com​](​https://google.com​)).
- As an active user I want to see a list of my links, ordered by creation date.
- As an active user I want to click on my links to see details and stats.

      AC:
        - I want to see how many times my link was clicked.
        - I want to see a list of different devices and user agents and percentages of access.

- There must be a README that explains how to set up the application and the algorithm used for generating the URL shortcode.

- As an active user I want an API key to access and integrate any other platform with this shortener.

      AC:
        - I want an endpoint to access all my links.
        - All endpoint results must be paginated.
        - I want an endpoint to shorten new URLs.

- You need to test all your code with RSpec.


> \* Research and understand how [Bit.ly](http://bit.ly) and [TinyURL](https://tinyurl.com/) work before you decide on how to generate URLs of the shortest possible length.
There must be a view for the Top 100 most frequently accessed URLs.
