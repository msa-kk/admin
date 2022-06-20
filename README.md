# admin

## How to install

1. Follow [instructions to create the GitHub App](https://github.com/github/safe-settings#how-to-use)
2. Take the environment variables from `.env` file to use them in the k8s deployment.
   1. Non-sensitive configuration can be set in the [k8s deployment file][k8s-deployment].
   2. Sensitive configuration can be set as a k8s secret and used in the [k8s deployment file][k8s-deployment].
3. Update the `Webhook URL` with the URL on k8s at <https://github.com/organizations/public-acme/settings/apps/safe-settings-public-acme>. Use the URL set in the [k8s ingress file](apps\safe-settings\deploy\k8s\ingress.yaml).
4. Deploy the `safe-settings` app on k8s with the [deploy workflow](.github\workflows\deploy-safe-settings.yml).

[k8s-deployment]: apps\safe-settings\deploy\k8s\deployment.yaml


