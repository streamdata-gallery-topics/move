---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Move Address To Vpc
  version: 1.0.0
  description: Moves an Elastic IP address from the EC2-Classic platform to the EC2-VPC
    platform.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=MoveAddressToVpc:
    get:
      summary: Move Address To Vpc
      description: Moves an Elastic IP address from the EC2-Classic platform to the
        EC2-VPC platform.
      operationId: moveaddresstovpc
      x-api-path-slug: actionmoveaddresstovpc-get
      parameters:
      - in: query
        name: AllocationId
        description: '[EC2-VPC] The allocation ID'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: PublicIp
        description: '[EC2-Classic] The Elastic IP address'
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Address
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---