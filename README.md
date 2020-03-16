# ZephroC's Library Services
This is mostly a toy project for playing with the single repository idea for micro-services.

It will eventually be a set of micro-services plus infrastructure (DBs and the like), that can all be run from a single root. Then acceptance tests can run against them as a whole.

It's also a blatant excuse to mess around with a variety of programming languages and tools in one place.

A library was picked as it's a nice public service institution which is kind of under threat these days, plus I really love books.

## Planned Features
- A metadata repository. Storing ISBNs, authors, covers etc.
- An API around that which is read focused, as you probably don't update book metadata much.
  - So it can utilise caching (probably Redis).
  - Basic CRUD operations
  - Can do searches etc.
- Some sort of ordering/ingest for when stock is bought/sold. Which implies some kind of stock DB that needs to be transactional.
- Reserving/checking out service which relates to the above.
- Eventually a UI, but I'm more backend focused.
- Possibly something to do with user reviews or tagging for surfacing interesting data not based directly on a books metadata.

## Left out features
Due to it being a toy project to run on my computer, adding security, admin roles, versioning will probably be left out.
Actually do some work.
