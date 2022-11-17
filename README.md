# 100K Fake US People Profiles Dataset

This database was primarily created for testing purposes.

The SQLite database contains the following columns:

```sql
  "id"          INTEGER,
  "first_name"  TEXT UNIQUE,
  "last_name"   TEXT UNIQUE,
  "gender"      TEXT,
  "job_title"   TEXT,
  "street"      TEXT UNIQUE,
  "city"        TEXT,
  "state"       TEXT,
  "zip"         TEXT,
  "company"     TEXT UNIQUE,
  "phone"       TEXT UNIQUE,
```

> Columns `first_name` and `last_name` are sorted by popularity

> The `street` address column does not represent an actual physical location rather, it is the result of the concatenation of randomly pulled plausible house number and randomly pulled plausible street name.

> Columns `city`, `state` and `zip` are pulled together randomly from United States ZIP Codes database

# Sources

- **First Name** - [Popular Baby Names - US Social Security](https://www.ssa.gov/oact/babynames/limits.html)
- **Last Name** - [United States Census Bureau](https://www.census.gov/topics/population/genealogy/data/2010_surnames.html)
- **Job Title** - [Bureau of Labor Statistics of the USA](https://www.bls.gov)
- **Street** - [OpenAddresses](https://openaddresses.io)
- **City, State and Zip** - [United States Postal Service](https://www.usps.com)
- **Company and Phone** - [Faker NPM library](https://fakerjs.dev/api/company.html#name)
