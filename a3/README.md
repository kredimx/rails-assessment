# Part II

## Invoices management

This is the [Rails starter code](https://github.com/kredimx/rails-assessment/tree/main/a3) for take-home assessments.

### Take-home assessment

#### * User stories
- As an authenticated User, I want to create invoices
so that I can add custom invoices.

- As an authenticated User, I want to edit invoices
so that I can correct any invoice data.

- As an authenticated User, I want to remove invoices
so that I can discard unnecessary invoices.

- As an authenticated User, I want to see the list of all the created/uploaded invoices
so that I can found invoices easily.
Acceptance criteria:
  - The user should be able to filter invoices by status, emitter, receiver and amount range

- As an authenticated User, I want to see a list of all the invoices I have received from a provider(emitter)
  - The user should be able to filter invoices by issue date (emitted_at)
  - The user should be able to see the total amount of the filtered list

- As an authenticated User, I want to import a set of XML that contain invoices
so that I can see the invoice data in the database.
Acceptance criteria:
  - The user should be able to upload hundreds of files at a time (extract the ZIP file `public/20220811012132-invoices.zip` to see the XML format and test with that batch of XML files)
  - If you need to create more XML files, after extracting the zip run this task `rake xml:generate_invoice` to generate more XML files within that same extracted directory `public/20220811012132-invoices/`
  - Hint: take a look at active_support’s `Hash.from_xml`

- As an authenticated User, I want to have an endpoint that renderizes the image of invoice `cfdi_digital_stamp` as QR

#### * Observations
- A user is a invoice receiver and is able to upload invoices
- This Rails app was created for only API.

#### * Objectives
- Sample data. We want to be able to run the app and see how it works.
- A reasonable architecture. No need to tune performance, but use best practices of...
  - software design: design principles (SOLID) and design patterns
  - performance: like paging, avoiding n+1 queries, background processing, etc. where you think it makes sense.
- Testing, it is very important for us to see that you understand how to test Ruby on Rails code.
- Well-organized code and following conventions (`rubocop`)
- The code doesn't need to be perfect, but aim for good readability.

#### * Delivery instructions
- Fork the Github repository (at this time, we will know that you have started the evaluation).
- Write us any question, or doubt responding the e-mail message.
- Delivery:
  - If you implemented API only, use Postman, or any other similar
  - Optional: use a client app or use Rails to render server and client side
  - Bonus: online. You can use Heroku, or any other similar
- After you have submitted the project, share to us the forked repository and we will schedule an interview with one of our engineers to review it with you.

### Project setup

- Ruby version: 3.1.0
- PostgreSQL (at least version 9.3 installed)
- Configuration: You can use any container manager such as Docker, or setup directly in your local.
