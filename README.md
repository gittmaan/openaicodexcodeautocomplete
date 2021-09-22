# OpenAI Codex Code Autocomplete README

"OpenAI Codex Code Autocomplete" extension helps connect to Codex API provided you have access to Codex API and have API KEY .

You can get the extension [at marketplace here](https://marketplace.visualstudio.com/items?itemName=OpenAICodexCodeAutoComplete.openaicodexcodeautocomplete)

## Features

- [OpenAI-Codex](https://openai.com/blog/openai-codex/)

## Requirements

- You must have a Codex API key.

## Usage

One of the way you can test the output is open a new file and write below code

```
Convert from Python to Javascript

Python:
def order(side, quantity, symbol, order_type=ORDER_TYPE_MARKET):
    try:
        print("sending order")
        order = client.create_order(
            symbol=symbol, side=side, type=order_type, quantity=quantity)
        print(order)
    except Exception as e:
        print("an exception occured - {}".format(e))
        return False

    return True

JavaScript:

```

You should get output similar to

```
Convert from Python to Javascript

Python:
def order(side, quantity, symbol, order_type=ORDER_TYPE_MARKET):
    try:
        print("sending order")
        order = client.create_order(
            symbol=symbol, side=side, type=order_type, quantity=quantity)
        print(order)
    except Exception as e:
        print("an exception occured - {}".format(e))
        return False

    return True

JavaScript:

function order(side, quantity, symbol, order_type=ORDER_TYPE_MARKET) {
    try {
        console.log("sending order");
        order = client.create_order(
            symbol=symbol, side=side, type=order_type, quantity=quantity);
        console.log(order);
    } catch (e) {
        console.log("an exception occured - {}".format(e));
        return false;
    }

    return true;
}

```
