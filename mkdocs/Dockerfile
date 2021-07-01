FROM python:3.9.2-alpine3.13

RUN apk add --no-cache gcc musl-dev git

COPY ./requirements.txt .
RUN pip install -r requirements.txt

WORKDIR /docs

ENTRYPOINT ["mkdocs"]
# This needs to be run in host network mode to work
CMD ["serve", "--dev-addr=127.0.0.1:8000"]
