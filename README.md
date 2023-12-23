# Goal: Building a JSON Parser

JSON (which stands for JavaScript Object Notation) is a lightweight data-interchange format, which is widely used for transmitting data over the Internet. It is formally defined by the IETF here: <https://tools.ietf.org/html/std90> or there’s a simpler graphical representation here: <https://www.json.org/json-en.html>

## Step 1

In this step, we will parse a valid simple JSON object, specifically: "{}", and an invalid JSON file and report which is which.
The goal is to build a minimalistic lexer and parser for this step.

The program should report to the standard output stream a suitable message and exit with the code 0 for valid and 1 for invalid. It is conventional for CLI tools to return 0 for success and between 1 and 255 for an error and allows us to combine CLI tools to create more powerful programs.

We will use the folder `tests/step1` to test our code.

## Step 2

Our next goal is to extend the parser to parse a simple JSON object containing string keys and string values.

```json
{"key": "value"}
```

We will use the folder `tests/step2` to test our code.

## Step 3

In this step your goal is to extend the parser to parse a JSON object containing string, numeric, boolean and null values, i.e.:

```json
{
  "key1": true,
  "key2": false,
  "key3": null,
  "key4": "value",
  "key5": 101
}
```

We will use the folder `tests/step3` to test our code.

## Step 4

In this step, we will extend the parser to parse a JSON object with object and array values.

```json
{
  "key": "value",
  "key-n": 101,
  "key-o": {},
  "key-l": []
}
```

We will use the folder `tests/step4` to test our code.

## Step 5

In this step, we will add some more tests to ensure that the parser can handle valid JSON and will fail with useful error messages on invalid JSON.
We will use the folder `tests/step5` to test our code. These tests are provided by `http://www.json.org/JSON_checker/test.zip`.
