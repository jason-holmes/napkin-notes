## Notation

term | definition
----|-------------
CC  | Concept Coach
SPE | Spaced Practice Exercise

## Tutor Ingests Book and Exercise Tag Map

## Tutor will have Special CC-Specific Courses

## Tutor Generates and Stores Per-Period CC Codes

`OX Tutor` will need to
generate and store
a per-`Period` `CC` `registration codes`
for each `CC-Specific Course`.

These codes will need to be made available
to third parties
for distribution to teachers and students.

## Tutor CC Plugin

Certain `Cnx` `Pages` will contain
a `OX Tutor` `CC plugin`
(some javascripty something or other)
which will present
`OX Tutor`-generated content
to `Cnx` users.

The `CC plugin` will be given
the current logged-in `User` (if any)
and the `Book:Page` associated with the current URL.
That information will be passed on to `OX Tutor`.

#### Anonymous User Visits CC Page URL

If an anonymous (not logged in) user
visits a `Cnx` `Page` with a `CC plugin`,
the `CC plugin` will display a login screen.

#### Logged in User Visits CC Page URL

If a logged in `User`
visits a `Cnx` `Page` with a `CC plugin`,
the `CC plugin` display will depend
on whether or not `OX Tutor` can associate the combination
of `User` and `Book:Page` URL
with a `Student` in a `CC-Specific Course`.

##### `User`/`Book:Page` Combo Identifies a `Student`

`OX Tutor` will create
a `CC` `Task` for the `Book:Page`
for the current `Student`.
This new `Task` will be displayed
in the `CC plugin`.

The first assessment of the `Task`
will be shown and be workable
by the `Student`.

##### `User`/`Book:Page` Combo Does NOT Identify a `Student`

If the `User`/`Book:Page` combination
does NOT identify a `Student`
in a `CC-Specific Course`,
the `CC plugin` will display
a place to enter a `registration code`.

Upon receipt of the
`User`/`Book:Page`/`registation code` triple,
`OX Tutor` will create a new `Student`
in the appropriate `Period`
of the `CC-Specific Course`
associated with the `registration code`.

Now that `OX Tutor`
can identify the `Student`,
the previous workflow
can be followed.

## Student Completes First Concept Coach Exercise for a Given Page

Upon the completion of the first `CC` `Task` assessment,
`OX Tutor` will
add the current `Task` to the `Student's` event history
(setting the `history_time`)
and populate its `SPE` placeholders (if any).

## Student Scores (Online and Download)