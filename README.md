# Homebank 2

Homebank 2 is the second, better written (though three years old and still poorly written) version of Homebank.

Unfortunately, I originally didn't set up a Git repository for this project, so there isn't any progress-tracking data available.

This repository contains both the [server](src/packages/server) and [client](src/packages/web) code.

## Server Structure

| Name                      | Description                                                          |
| ------------------------- | -------------------------------------------------------------------- |
| [api](src/packages/server/api)          | REST API routes for managing and retrieving data |
| [auth](src/packages/server/auth)     | Authentication, permissions, and queries for authentication                                    |
| [config](src/packages/server/config)         | Access keys for the database                                      |
| [crypto](src/packages/server/crypto)   | Password and identification cryptographic utility functions                                            |
| [db](src/packages/server/db)     | Database models and controllers                                     |
| [lib](src/packages/server/lib)      | Utility functions for the server                     |

## Client Structure

The client is a typical Next.JS application, containing [components](src/packages/web/components) used commonly between pages, [pages](src/packages/web/pages) allowing control of specific data, [static files](src/packages/web/public), in this case images, and [CSS style sheets](src/packages/web/styles).

## Improvements from Version 1

As my first attempt at a full-stack web application, Homebank 1 was a poorly designed and executed program.

12-year-old me had no problem with one 3000-line "index.js" controlling the whole application. It worked, but it was a mess to maintain. It also lacked type-checking and basic security features like query sanitization.

These shortcomings motivated 13-year-old me to create this version. I was still new to Node.JS, but I had some better ideas about file structure, database management, and how to set up a REST API. Though it doesn't always follow best practices, it's a significant improvement.

I've come a long way from the Homebank project, but I still like looking back from time to time on how I started seriously programming. Homebank remains of my favorites from this time period.