# solhint-plugin-custom-functions-order

## Setup

First install the necessary packages:

```
npm install --save-dev solhint lmcorbalan/solhint-plugin-custom-functions-order
```

Then add a `.solhint.json` configuration file:

```json
{
  "plugins": ["custom-functions-order"],
  "rules": {
    "custom-functions-order/custom-ordering": [
      "warn",
      {
        "functionsOrder": [
          "external view",
          "external pure",
          "public view",
          "public pure",
          "external",
          "public",
          "internal",
          "internal view",
          "internal pure",
          "private",
          "internal view",
          "internal pure"
        ]
      }
    ]
  }
}
```
