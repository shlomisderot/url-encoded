# url-encoded
Convert urlencoded string ('application/x-www-form-urlencoded') into valid Javascript literal object (JSON format).

The purpose of this library is to take urlencoded string such as: 
```
'protocol=echo-protocol&topic=assets%3Aremove&data=%7B%22uid%22%3A%22bd17ecad-fc2e-4568-ae21-ad08ddf48b59%22%2C%22gid%22%3A%221a71d70d-bc5b-46f1-b6ec-16776b6285eb%22%2C%22data%22%3A%7B%22id%22%3A%225c1116adc9c31f74efcdafbe%22%7D%7D'
```

And convert it to Javascript literal object such as: 
```
{
  data: {
  product_id: "5c1116adc9c31f74efcdb022",
      group_id: "1a71d70d-bc5b-46f1-b6ec-16776b6285eb",
      user_id: "bd17ecad-fc2e-4568-ae21-ad08ddf48b59"

  },
  protocol: "echo-protocol",
  topic: "assets:remove"
}
```

### Running example:
Assuming NodeJS already installed on the machine, get into the url-encoded and run:  ``` node index.js ```

To get more information read [parse urlencoded string-json in one line code](https://www.linkedin.com/pulse/parse-urlencoded-string-json-one-line-code-shlomi-elbaz/)
