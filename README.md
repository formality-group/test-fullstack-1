copy .env.example to .env

exec `docker run -it --rm -v ``pwd``:/app -p 3000:3000 -w /app node:24 bash`

within this container;
* exec: `npm i`
* exec: `npm run db:push`
* exec: `npm run dev`

open http://localhost:3000 => it should work!
