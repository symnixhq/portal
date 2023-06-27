---
# reference: https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests
name: "Service Deployment"
description: "Add your service which should be deployable next here"
title: "Make [SERVICE] ready for Deployment"
labels: [
  "new-service"
]
assignees: xFuture603

body:
  - type: markdown
    attributes:
      value: |
        Requesting a new deployable service follows some simple rules:

        - **Check** if the service is already requested or deployable
        - **Explain** the criteria to fulfill your service request
        - **Add** more details like links to the software, links to the docker image 
        - **Follow Up** in the discussion to your service request

  - type: textarea
    id: service_name
    attributes:
      label: "Service name"
      description: Please add the name of the software you want to deploy.
      placeholder: Name of the service you want to deploy. For example: < nextcloud >
    validations:
      required: true

  - type: textarea
    id: resources
    attributes:
      label: "Resources"
      description: Please provide some additional information about the service. For example:
      placeholder: Links to the official repository, link to the docker image, link to the official service website
    validations:
      required: false
