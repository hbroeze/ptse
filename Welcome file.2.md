## Example database
```mermaid
classDiagram
class countries {
continent: string
country : string
}
class codes {
country : string
code: string
}
codes --< countries
```
## Tables
### countries
|continent | country |
|--|--|
|Europe  | Germany |

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTUyNjkyNzE5MSwtMzMyNDU1MzYzXX0=
-->