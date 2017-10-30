## Define a custom type
```type dict_val = int * string;;```

## Create a list with values of this type
```let underwood_kids = [(1,"Taka");(2,"Toshi");(3,"Miyo")];;```

```let rec get_name (lst: dict_val list) (k: int): string option =
match lst with | [] -> None
| (k',v)::tl -> if k = k' then (Some v) else getName tl k;;
```

```
val get_name : dict_val list -> int -> string option = <fun>
```
