# SpotMe

Car parking and space renting web application that connects drivers with
homeowners.

The motivation for this application comes from the dual problem of finding
parking in congested metropolitan areas, as well as lost income potential from
unused parking spaces.

## Built With

- Frontend
  - Handlebars.js
  - Bootstrap
- Backend
  - Node.js
  - Express.js
- Database Layer
  - PostgreSQL & PostGIS
  - Sequelize ORM
- Other
  - Google Maps API

### Running the application

1) Clone the repository
```bash
git clone https://github.com/herman-ho/spotme.git
```

2) Switch to working directory
```bash
cd spotme
```

3) Install node dependencies
```bash
npm install
```

4) Run database migrations (optional: seeds)
```bash
sequelize db:migrate && sequelize db:seed:all
```

5) Place Google Maps Streetview API key in handlebars partial

`views/partials/api-key-streetview.handlebars`

6) Run application, listening on `localhost:8000`
```bash
npm start
```
