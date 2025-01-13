`docker run -it --rm -v `pwd`:/app -p 3000:3000 node:22 bash`
npm i
npm run db:push
npm run dev
