# 🚀 action-repo

This is a demonstration repository to trigger GitHub webhook events such as:

- ✅ Push
- ✅ Pull Request
- ✅ Merge (as bonus)

These events are configured to be sent to a webhook receiver (`webhook-repo`) which stores them in a MongoDB database and displays them on a live UI.

## 🧩 How It Works

Any of the following actions in this repository will trigger a webhook to the receiver:

1. **Push** – pushing any commit to a branch
2. **Pull Request** – opening a pull request from one branch to another
3. **Merge** – merging an approved pull request

## 🔧 Webhook Configuration

To configure the webhook:

1. Go to **Settings → Webhooks**
2. Click **Add webhook**
3. Use the following details:
   - **Payload URL:** `https://<your-webhook-server>/webhook`
   - **Content type:** `application/json`
   - **Secret:** *(leave blank or use a predefined one)*
   - **Events:** Select:
     - ✅ Push
     - ✅ Pull requests

## 🧪 Sample Trigger Actions

- Make a new branch and push a commit
- Open a pull request from that branch to `main`
- Merge the pull request (bonus merge event)

## 📎 Related Repo

👉 [webhook-repo](https://github.com/SahdevPrajapati18/webhook-repo)
