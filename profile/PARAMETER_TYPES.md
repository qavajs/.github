## Parameter types
               
The framework support all cucumber types

| Parameter Type | Description                                                                                                                                                                                                                                                                                                       |
|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `{int}`        | Matches integers, for example `71` or `-19`. Converts to a 32-bit signed integer if the platform supports it.                                                                                                                                                                                                     |
| `{float}`      | Matches floats, for example `3.6`, `.8` or `-9.2`. Converts to a 32 bit float if the platform supports it.                                                                                                                                                                                                        |
| `{word}`       | Matches words without whitespace, for example `banana` (but not `banana split`).                                                                                                                                                                                                                                  |
| `{string}`     | Matches single-quoted or double-quoted strings, for example `"banana split"` or `'banana split'` (but not `banana split`). Only the text between the quotes will be extracted. The quotes themselves are discarded. Empty pairs of quotes are valid and will be matched and passed to step code as empty strings. |
| `{}` anonymous | Matches anything (`/.*/`).                                                                                                                                                                                                                                                                                        |
| `{bigdecimal}` | Matches the same as `{float}`, but converts to a `BigDecimal` if the platform supports it.                                                                                                                                                                                                                        |
| `{double}`     | Matches the same as `{float}`, but converts to a 64 bit float if the platform supports it.                                                                                                                                                                                                                        |
| `{biginteger}` | Matches the same as `{int}`, but converts to a `BigInteger` if the platform supports it.                                                                                                                                                                                                                          |
| `{byte}`       | Matches the same as `{int}`, but converts to an 8 bit signed integer if the platform supports it.                                                                                                                                                                                                                 |
| `{short}`      | Matches the same as `{int}`, but converts to a 16 bit signed integer if the platform supports it.                                                                                                                                                                                                                 |
| `{long}`       | Matches the same as `{int}`, but converts to a 64 bit signed integer if the platform supports it.                                                                                                                                                                                                                 |

Additionally, framework adds own types to work with framework libraries

 | Parameter Type | Description                                                                                 |
|----------------|---------------------------------------------------------------------------------------------|
| `{element}`    | Matches element alias (e.g 'Search > Input') that then will be resolved to wdio element     |
| `{text}`       | Matches string that may be memory identifier (e.g '$username') and resolves correspondingly |
 | `{validation}` | Matches string that resolves into function to validate passed values                        |

