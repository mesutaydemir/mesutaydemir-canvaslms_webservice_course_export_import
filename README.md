# CANVAS LMS COURSE EXPORT

## List active courses in an account
We are getting course **id** `GET https://CANVAS_URL/api/v1/accounts/:account_id/courses` by providing **account_id_**
## Content Export
Provide **course_id**`POST https://CANVAS_URL/api/v1/courses/:course_id/content_exports` and export content. Get **id**

## Show Content Export
Provide **course_id** and **id** `GET https://CANVAS_URL/api/v1/courses/:course_id/content_exports` and get **url** aunder **attachment**


# CANVAS LMS COURSE IMPORT
## List active courses in an account
Provide **account_id_**  GET `https://CANVAS_URL/api/v1/accounts/:account_id/courses` and get course **id**.

## Create Content Migration
Provide **course_id**, **settings[file_url]** and **migration_type** POST `https://CANVAS_URL/api/v1/courses/:course_id/content_migrations`  and start migration:

```ruby
**course_id** = **id**
**settings[file_url]** = **url**
**migration_type** = canvas_cartridge_importer
```
