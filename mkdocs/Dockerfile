FROM python:3.9.2-alpine3.13

RUN apk add --no-cache gcc musl-dev

COPY ./requirements.txt .
RUN pip install -r requirements.txt

WORKDIR /docs

EXPOSE 8000

ENTRYPOINT ["mkdocs"]
CMD ["serve", "--dev-addr=0.0.0.0:8000"]
