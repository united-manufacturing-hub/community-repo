# addPrefix

This is a subflow that can add prefixes to JSON objects, and also remove the timestamp if required. It was contributed to the community by an individual named DanielH.

## Usage
1. Import the `addPrefix` subflow into your Node-RED instance.
2. Configure the subflow by setting the following environment variables:
    - `prefix`: The prefix that you want to add to your JSON objects.
    - `cTime`: A boolean value that determines whether to keep the timestamp unchanged (true) or not (false).
    - `rTime`: A boolean value that determines whether to remove the timestamp (true) or not (false).
3. Connect the input of the subflow to the JSON object that you want to add prefixes to.
4. Connect the output of the subflow to the node that will process the modified JSON object.

## Example
Suppose you have a JSON object with the following structure:

```js
{
"name": "John",
"age": 30,
"city": "New York",
"timestamp_ms": 1646834200000
}
```

If you want to add the prefix "myPrefix" to this object and keep the timestamp unchanged, you can configure the subflow as follows:

- `prefix`: myPrefix
- `cTime`: true
- `rTime`: false

After processing the object through the subflow, the output will look like this:
```js
{
"myPrefix_name": "John",
"myPrefix_age": 30,
"myPrefix_city": "New York",
"timestamp_ms": 1646834200000
}
```

If you want to remove the timestamp from the object, you can configure the subflow as follows:

- `prefix`: myPrefix
- `cTime`: false
- `rTime`: true

After processing the object through the subflow, the output will look like this:
```js
{
"myPrefix_name": "John",
"myPrefix_age": 30,
"myPrefix_city": "New York"
}
```
You can customize the prefix and timestamp options as per your requirements.

You can copy the template for this subflow from [here](./addPrefix.json).
