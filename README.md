# azure_aaa


gcloud iam service-accounts add-iam-policy-binding "${SERVICE_ACCOUNT}" \
  --project="${PROJECT_ID}" \
  --role="roles/iam.workloadIdentityUser" \
  --member="principalSet://iam.googleapis.com/${WORKLOAD_IDENTITY_POOL_ID}/attribute.repository/${GitHubユーザー名}/${リポジトリ名}"

[class method aws github](https://dev.classmethod.jp/articles/allowing-assumerole-only-for-specific-repositories-and-branches-with-oidc-collaboration-between-github-actions-and-aws/)
