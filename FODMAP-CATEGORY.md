### Create catalog

```bash
ask smapi create-interaction-model-catalog --catalog-name fodmap-category
```

```json
{
  "catalogId": "amzn1.ask.interactionModel.catalog.f938500f-7979-4a57-b329-d9f71ed8cd91"
}
```

### Create a catalog version

```bash
ask smapi create-interaction-model-catalog-version \
--catalog-id amzn1.ask.interactionModel.catalog.f938500f-7979-4a57-b329-d9f71ed8cd91 \
--source-url https://raw.githubusercontent.com/pedrozc90/ast/master/fodmap-category-types.json \
--source-type URL
```

### Check progress

```bash
ask smapi get-interaction-model-catalog-update-status \
--catalog-id amzn1.ask.interactionModel.catalog.f938500f-7979-4a57-b329-d9f71ed8cd91 \
--update-request-id f938500f-7979-4a57-b329-d9f71ed8cd91-Time-2024-05-11T16-09-10.893 \
--profile default
```

```json
{
  "lastUpdateRequest": {
    "errors": [],
    "status": "SUCCEEDED",
    "version": "1"
  }
}
```
