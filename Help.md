logsBucket: 'gs://your-custom-bucket-name'


gcloud projects add-iam-policy-binding project-79dcfebc-a5e4-4f53-973  --member="serviceAccount:316946743158-compute@developer.gserviceaccount.com"  --role="roles/logging.logWriter"


gcloud container clusters get-credentials gcp-devops-project --zone us-central1-a --project kodekloud-gcp-training



# Find your PROJECT_ID if you don't know it
gcloud config get-value project

# Full command with your real project ID — example:
gcloud projects add-iam-policy-binding gcpdevops-project \
  --member="serviceAccount:316946743158-compute@developer.gserviceaccount.com" \
  --role="roles/logging.logWriter"

# You should see output like:
# Updated IAM policy for project [gcpdevops-project].
# bindings:
# - members:
#   - serviceAccount:316946743158-compute@developer.gserviceaccount.com
#   role: roles/logging.logWriter



gcloud container clusters get-credentials gcp-devops-project --zone us-central1-a --project project-79dcfebc-a5e4-4f53-973


kubectl get namespace

kubectl create namespace gcp-devops-prod

kubectl get namespace

After deployment completed into GCP

kubectl get pods

kubectl get namespace

kubectl get pods -n gcp-devops-prod