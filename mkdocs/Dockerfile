FROM python:3.9.2-alpine3.13

RUN pip install mkdocs mkdocs-material mkdocs-monorepo-plugin mkdocs-versioning

WORKDIR /docs

EXPOSE 8000

ENTRYPOINT ["mkdocs"]
CMD ["serve", "--dev-addr=0.0.0.0:8000"]
