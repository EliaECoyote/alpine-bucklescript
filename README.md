# Alpine-bucklescript

Bucklescript on a node-alpine image. Ready to use for OCaml / ReasonML projects that target javascript.

---

## Supported tags and respective Dockerfile links

- [`7`, `7.2`, `7.2.2`, `latest`](https://github.com/EliaECoyote/alpine-bucklescript/blob/v7.2.2/7/Dockerfile)
- [`7.1`, `7.1.1`](https://github.com/EliaECoyote/alpine-bucklescript/blob/v7.1.1/7/Dockerfile)

---

## Usage

```Docker
FROM eliaecoyote/alpine-bucklescript:7

WORKDIR /home/node/app

COPY your_project ./

RUN npm link "bs-platform" && yarn bsb -make-world
```

---

MIT licensed.

```txt
THIS DOCKER IMAGE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE MAINTAINERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE DOCKER IMAGE OR THE USE OR OTHER DEALINGS IN THE DOCKER IMAGE.
```

---

CI/CD managed by *docker automated builds* service.

Track an [issue on github](https://github.com/EliaECoyote/alpine-bucklescript/issues).
