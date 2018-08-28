swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PurchaseScheduledInstances:
    get:
      summary: Purchase Scheduled Instances
      description: Purchases one or more Scheduled Instances with the specified schedule.
      operationId: purchasescheduledinstances
      x-api-path-slug: actionpurchasescheduledinstances-get
      responses:
        200:
          description: OK
      tags:
      - Scheduled Instance
  /?Action=RunScheduledInstances:
    get:
      summary: Run Scheduled Instances
      description: Launches the specified Scheduled Instances.
      operationId: runscheduledinstances
      x-api-path-slug: actionrunscheduledinstances-get
      parameters:
      - in: query
        name: CidrIp
        description: The CIDR IPv4 address range
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: FromPort
        description: The start of port range for the TCP and UDP protocols, or an
          ICMP type number
        type: string
      - in: query
        name: GroupId
        description: The ID of the security group
        type: string
      - in: query
        name: IpPermissions.N
        description: A set of IP permissions
        type: string
      - in: query
        name: IpProtocol
        description: The IP protocol name or number
        type: string
      - in: query
        name: SourceSecurityGroupName
        description: The name of a destination security group
        type: string
      - in: query
        name: SourceSecurityGroupOwnerId
        description: The AWS account number for a destination security group
        type: string
      - in: query
        name: ToPort
        description: The end of port range for the TCP and UDP protocols, or an ICMP
          type number
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scheduled Instances
  /?Action=DescribeScheduledInstances:
    get:
      summary: Describe Scheduled Instances
      description: Describes one or more of your Scheduled Instances.
      operationId: describescheduledinstances
      x-api-path-slug: actiondescribescheduledinstances-get
      responses:
        200:
          description: OK
      tags:
      - Scheduled Server Instances
  /?Action=DescribeScheduledInstanceAvailability:
    get:
      summary: Describe Scheduled Instance Availability
      description: Finds available schedules that meet the specified criteria.
      operationId: describescheduledinstanceavailability
      x-api-path-slug: actiondescribescheduledinstanceavailability-get
      responses:
        200:
          description: OK
      tags:
      - Server Instance Availability