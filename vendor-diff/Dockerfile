FROM python:3-alpine

LABEL "maintainer"="Kim Ngo <akngo16@gmail.com>"
LABEL "repository"="https://github.com/findkim/go-mod-github-actions"
LABEL "version"="0.1.0"

LABEL "com.github.actions.name"="vendor diff"
LABEL "com.github.actions.description"="Verify vendor is up to date with go mod"
LABEL "com.github.actions.icon"="circle-check"
LABEL "com.github.actions.color"="blue"

RUN apk --no-cache add jq curl

COPY vendor-diff.py entrypoint.sh ./
ENTRYPOINT [ "./entrypoint.sh" ]
