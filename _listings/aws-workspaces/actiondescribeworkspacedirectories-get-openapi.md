---
swagger: "2.0"
x-collection-name: AWS WorkSpaces
x-complete: 0
info:
  title: AWS WorkSpaces Service API Describe Workspace Directories
  version: 1.0.0
  description: Retrieves information about the AWS Directory Service directories in
    the region that are registered with Amazon WorkSpaces and are available to your
    account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateTags:
    get:
      summary: Create Tags
      description: Creates tags for a WorkSpace.
      operationId: createTags
      x-api-path-slug: actioncreatetags-get
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID of the request
        type: string
      - in: query
        name: Tags
        description: The tags of the request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=CreateWorkspaces:
    get:
      summary: Create Workspaces
      description: Creates one or more WorkSpaces.
      operationId: createWorkspaces
      x-api-path-slug: actioncreateworkspaces-get
      parameters:
      - in: query
        name: Workspaces
        description: An array of structures that specify the WorkSpaces to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""
  /?Action=DeleteTags:
    get:
      summary: Delete Tags
      description: Deletes tags from a WorkSpace.
      operationId: deleteTags
      x-api-path-slug: actiondeletetags-get
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID of the request
        type: string
      - in: query
        name: TagKeys
        description: The tag keys of the request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=DescribeTags:
    get:
      summary: Describe Tags
      description: Describes tags for a WorkSpace.
      operationId: describeTags
      x-api-path-slug: actiondescribetags-get
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID of the request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=DescribeWorkspaceBundles:
    get:
      summary: Describe Workspace Bundles
      description: Obtains information about the WorkSpace bundles that are available
        to your account in the specified region.
      operationId: describeWorkspaceBundles
      x-api-path-slug: actiondescribeworkspacebundles-get
      parameters:
      - in: query
        name: BundleIds
        description: An array of strings that contains the identifiers of the bundles
          to retrieve
        type: string
      - in: query
        name: NextToken
        description: The NextToken value from a previous call to this operation
        type: string
      - in: query
        name: Owner
        description: The owner of the bundles to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspace Bundles
  /?Action=DescribeWorkspaceDirectories:
    get:
      summary: Describe Workspace Directories
      description: Retrieves information about the AWS Directory Service directories
        in the region that are registered with Amazon WorkSpaces and are available
        to your account.
      operationId: describeWorkspaceDirectories
      x-api-path-slug: actiondescribeworkspacedirectories-get
      parameters:
      - in: query
        name: DirectoryIds
        description: An array of strings that contains the directory identifiers to
          retrieve information for
        type: string
      - in: query
        name: NextToken
        description: The NextToken value from a previous call to this operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspace Directories
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