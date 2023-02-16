# CANVAS LMS COURSE EXPORT

## List active courses in an account
`GET https://mergen.anadolu.edu.tr/api/v1/accounts/:account_id/courses` ile **account_id_** verip ders **id** değerini al.

## Content Export
`POST https://mergen.anadolu.edu.tr/api/v1/courses/:course_id/content_exports` ile **course_id** verip içeriği dışarı aktar. **id** değerini al.

## Show Content Export
`GET https://mergen.anadolu.edu.tr/api/v1/courses/:course_id/content_exports` ile **course_id** ve **id** değerlerini verip **attachment** altında **url** yi al.


# CANVAS LMS COURSE IMPORT
## List active courses in an account
GET `https://ozmergen.anadolu.edu.tr/api/v1/accounts/:account_id/courses` ile **account_id_** verip ders **id** değerini al.

## Create Content Migration
POST `https://ozmergen.anadolu.edu.tr/api/v1/courses/:course_id/content_migrations` ile **course_id** ve **settings[file_url]** ve **migration_type** değerleri girilip ders aktarım işlemi gerçekleştirilir:

```ruby
**course_id** = **id**
**settings[file_url]** = **url**
**migration_type** = canvas_cartridge_importer
```
