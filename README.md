# Insights all Along!

Any modern software written today depends on code from open source ecosystems.
In fact, Linux Foundation has estimated that 70-90% of the code in any modern
software is from open sources in form of libraries, frameworks, and tools. Have
you ever wondered whats inside these libraries?

## Problem

Build a [Nextjs 16](https://nextjs.org/blog/next-16) application that implements the user interface
as per the design in [this Figma Project](https://www.figma.com/design/25zhLiAxtNfTDc0e9pIzHr/SafeDep-Internship-Task?node-id=1-447).

The application should show details about an Open Source package at URL:

- `https://localhost:3000/p/{ecosystem}/{name}/{version}`
- Example URL: `https://localhost:3000/p/npm/nextjs/15.5.4`

The application must use:

- Nextjs 16.x
- Nextjs Server Actions (for fetching data about open source packages)
- Typescript
- Tailwind CSS
- Shadcn UI

For fetching data about open source packages, you will need to access SafeDep API. 
Sign-up for a free account at [app.safedep.io](https://app.safedep.io) to get an API key (refer to `Settings > API Keys`)

- Tenant ID (format: `<team>-<org>.safedep.io`)
- API Key

**Note:** Alternatively, you can sign-up using [vet](https://github.com/safedep/vet) from CLI by running `vet cloud quickstart` to obtain your `TenantID` and `API Key`.

Using `TenantID` and `API Key`, you can access SafeDep API to fetch the required data
about open source packages.

For your reference:

- See [insights-client](./insights-client), a Typescript example of how to use Insights API
- See [malysis-client](./malysis-client/), a Typescript example of how to use Malysis API
- See [insights-sample.json](./insights-sample.json) for an example response from Insights API, useful for mocking
- See [malysis-sample.json](./malysis-sample.json) for an example response from Malysis API, useful for mocking

**Note:** The data may not be available for all packages. Handle the error gracefully by displaying an appropriate error message.

### Submission Instructions

Follow the instructions below to submit your solution:

1. Create a public GitHub repository
2. Add the code implementing your solution to the repository
3. Share the repository URL with `jobs@safedep.io` with subject `[SWE-FE-Intern-2026]: Your Name`

**IMPORTANT:** Your repository should include a README.md file with the instructions to run the application.

## Questions?

Send email to `job@safedep.io`

## Troubleshooting

For any issue with [SafeDep API](https://docs.safedep.io/),
please reach out to `jobs@safedep.io` with the subject `[SafeDep API Issue]`.
