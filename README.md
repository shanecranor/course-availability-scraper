## Project Goals
- Learn Angular
- Use Docker
- Create and optimize a database
- Scrape course & course registration data for colleges using banner (hopefully without overloading their servers)
- Display information in a manner useful to students

## Initial thoughts on architecture
two services:
- rest or GQL api for the frontend
- entirely seperate scraping service that runs automatically and uploads to the database

use zod for data validation?

questions:
- What framework to use for the backend?
- Express? Nest.JS?

 starting with Express due to its easier learning curve
- orm vs raw sq?


going to try zapatos or kysely and see where it takes me

probably kysely first


how should we store time series data
- after research on a bunch of fancy time serires dbs, seems like that is way overkill
- instead we can just store the data more intelligently and instead of creating a new row if the the new row is identical to the old row, just increment a "valid to" date
- todo: see if this is a bad idea lmoa


 todo:
- finish docker container setup
  - setup postgres
  - finalize DB architecture
