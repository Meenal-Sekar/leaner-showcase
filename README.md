# Learner Showcase (MERN)
Sections: Projects, Testimonials, Placements, Achievements — filterable by Region (Kerala / Tamil Nadu / Telugu) and Course.

## Run
Needs Node 18+ and MongoDB (local or Atlas).

    cd server && cp .env.example .env && npm i && npm run seed && npm run dev   # API :5000
    cd client && npm i && npm run dev                                          # UI  :5173

## API
GET /api/:type?region=Kerala&course=MERN   (type = projects | testimonials | placements | achievements)
GET /api/meta/courses
POST/PUT/DELETE /api/:type[/:id]  — send header `x-admin-key: <ADMIN_KEY from .env>`
