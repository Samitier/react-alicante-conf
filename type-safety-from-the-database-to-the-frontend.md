# Type safety from the DB to the frontend

Speaker: Forbes Lindesay

## Introduction

We have types in a database, but we "lose them" in the FE whenever we use those db queries or we call APIs.

## Databases

He talks about generating types from db queries. Like the npm package `databases`, which automatically types the DB queries.

## API calls (GraphQL)

Generate Types automatically from GraphQL queries.

## API calls (in Typescript)

Create types as an npm package and add it as "references" in tsconfig.json. 
Or directly share types between front and backend if you happen to have both in the same repo.

## Internal API calls (not in Typescript)

He showed code for generating Types from a Rust backend.

## More examples about generating code

He showed an example about some JSON files with translation strings. He then proceed to generate a Type for those JSON files.
Basically a node script that reads the JSONs and lists the key strings and writes them in a file.
Then, interesting, uses prettier programmatically to format that generated file. Cool.

## Runtime validation

He uses `funtypes` package for that. Validates schemas and generates Typescript types from that.
Basically what Zod does.

## Ts-reset

Library that overrides some global TS types to improve them. For instance, it changes JSON.parse so that it returns `unknown` instead of `any`.

**Opinion**: about generating types from backend code, sadly no use for us. We can, however, share types between functions and apps. 
But generating types from a json file was pretty interesting and we could use that for translations, for instance. 
Regarding runtime validation, we are already using Zod for that.