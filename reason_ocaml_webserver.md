# ReasonML and OCaml

### Reason
```
let handler = (conn, req, body) => {
  print("Handling request: %s", req |> Request.uri |> Uri.path);
  Server.respond_string(~status=`Ok, ~body="Hello Reason!", ())
};
```

### Reason 1
Original: https://twitter.com/jlongster/status/919970735891894272

```
let handler conn req body => {
	print "Handling request: %s" (req |> Request.uri |> Uri.path);
	Server.respond_string status::`Ok body::"Hello Reason!" ()
};
```


### OCaml
```
let handler conn req body =
  print "Handling request: %s" ((req |> Request.uri) |> Uri.path);
  Server.respond_string ~status:`Ok ~body:"Hello Reason!" ()
```
