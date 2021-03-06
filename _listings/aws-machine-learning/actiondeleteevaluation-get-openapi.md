---
swagger: "2.0"
x-collection-name: AWS Machine Learning
x-complete: 0
info:
  title: AWS Machine Learning API Delete Evaluation
  version: 1.0.0
  description: Assigns the DELETED status to an Evaluation, rendering it unusable.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateEvaluation:
    get:
      summary: Create Evaluation
      description: Creates a new Evaluation of an MLModel.
      operationId: createEvaluation
      x-api-path-slug: actioncreateevaluation-get
      parameters:
      - in: query
        name: EvaluationDataSourceId
        description: The ID of the DataSource for the evaluation
        type: string
      - in: query
        name: EvaluationId
        description: A user-supplied ID that uniquely identifies the Evaluation
        type: string
      - in: query
        name: EvaluationName
        description: A user-supplied name or description of the Evaluation
        type: string
      - in: query
        name: MLModelId
        description: The ID of the MLModel to evaluate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Evaluations
  /?Action=DeleteEvaluation:
    get:
      summary: Delete Evaluation
      description: Assigns the DELETED status to an Evaluation, rendering it unusable.
      operationId: deleteEvaluation
      x-api-path-slug: actiondeleteevaluation-get
      parameters:
      - in: query
        name: EvaluationId
        description: A user-supplied ID that uniquely identifies the Evaluation to
          delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Evaluations
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