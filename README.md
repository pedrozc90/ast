# Alexa slot types

A collection of slot types for Alexa Skills.

## Usage

### Create a new catalog

```bash
ask smapi create-interaction-model-catalog --catalog-name foods
```

```json
{
  "catalogId": "amzn1.ask.interactionModel.catalog.de3b2ffc-5b60-4f26-bdb3-af60153d9934"
}
```

### Create a catalog version

```bash
ask smapi create-interaction-model-catalog-version \
--catalog-id amzn1.ask.interactionModel.catalog.de3b2ffc-5b60-4f26-bdb3-af60153d9934 \
--source-url https://raw.githubusercontent.com/pedrozc90/ast/master/food-types.json \
--source-type URL
```

### Check progress

```bash
ask smapi get-interaction-model-catalog-update-status \
--catalog-id amzn1.ask.interactionModel.catalog.de3b2ffc-5b60-4f26-bdb3-af60153d9934 \
--update-request-id de3b2ffc-5b60-4f26-bdb3-af60153d9934-Time-2024-05-07T02-55-17.433 \
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
