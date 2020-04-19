FROM alpine as build

RUN apk --no-cache --update add build-base make

WORKDIR /app
COPY . .
RUN make


FROM alpine

COPY --from=build /app/prime /app/prime

ENTRYPOINT ["/app/prime"]
