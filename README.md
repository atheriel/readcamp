# readcamp

**readcamp** is a simple R package to munge DataCamp's group exports into a tidy
format. It is useful for group administrators who wish to understand how their
students are doing, and prefer to perform this analysis in R.

## Usage

**readcamp** exposes one main function that reads all course & chapter grades
and completion information from the `.zip` archive downloaded from the DataCamp
website:

```r
readcamp::read_group_export("group_export_XXXX.zip")
```

This will return an object containing course- and chapter-level start and end
dates, grades, and completion.
