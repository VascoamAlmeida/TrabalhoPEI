# Local configuration

The BaseX RESTXQ modules intentionally contain **no MongoDB credentials or deployment URL**.

Before starting BaseX, define these environment variables:

- `MONGODB_DATA_API_KEY` — a valid MongoDB Atlas Data API key.
- `MONGODB_DATA_API_URL` — the MongoDB Atlas Data API `find` action endpoint used by the project.

Example endpoint shape (replace it with your own authorized deployment):

```text
https://<region>.aws.data.mongodb-api.com/app/<app-id>/endpoint/data/v1/action/find
```

## RESTXQ resources

- `/Vendas?year=2023&month=10`
- `/Refund?year=2023&month=10`
- `/StatsVendas?year=2023&month=10`
- `/StatsRefund?year=2023&month=10`
- `/StatsCliente`

The key that existed in the original academic submission was removed during portfolio preparation. If it still exists in Atlas, it should be revoked and replaced.
