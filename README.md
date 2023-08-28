# Build and deploy

Command to build the application. PLease remeber to change the project name and application name
```
gcloud builds submit --tag gcr.io/peaceful-terra-395212/streamlit-gcp  --project=peaceful-terra-395212
```

Command to deploy the application
```
gcloud run deploy --image gcr.io/peaceful-terra-395212/streamlit-gcp --platform managed  --project=<ProjectName> --allow-unauthenticated
```