## Deploying upload-data

```shell
gcloud functions deploy upload_data \
--gen2 \
--region=us-central1 \
--runtime=python312 \
--source=. \
--entry-point=2-upload-data \
--service-account=data-pipeline-robot-2024@musa-cloud.iam.gserviceaccount.com \
--memory=4Gi \
--timeout=240s \
--trigger-http \
--no-allow-unauthenticated
```