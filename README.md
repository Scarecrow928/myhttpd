## myhttpd

### build prerequisite

- cmake
- make
- boost >= 1.76
- libstdc++
- g++ or clang++
- docker (optional)

### build

- native: `cmake . && cmake --build . -j4`
- docker: `docker build -t <tag> .`
- docker-compose: `docker-compose build`

### run

- native: `./myhttpd`
- docker: `docker run -it -p 12000:12000 -v $(pwd)/html:/var/www/html <tag>`
- docker-compose: `docker-compose up`

### demo
- [direct](http://cn1.scarecrow928.com:12000)
- [behind reverse proxy](https://cn1.scarecrow928.com:10443/myhttpd)