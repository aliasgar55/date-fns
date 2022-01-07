# Serbian (sr) locale

## `format` and `parse`

| Title                           | Token string | Date                     | `format` result                                 | `parse` result           |
| ------------------------------- | ------------ | ------------------------ | ----------------------------------------------- | ------------------------ |
| Calendar year                   | yo           | 1987-02-11T12:13:14.015Z | 1987.                                           | 1987-01-01T00:00:00.000Z |
|                                 |              | 0005-01-01T12:13:14.015Z | 5.                                              | 0005-01-01T00:00:00.000Z |
| Local week-numbering year       | Yo           | 1987-02-11T12:13:14.015Z | 1987.                                           | 1986-12-29T00:00:00.000Z |
|                                 |              | 0005-01-01T12:13:14.015Z | 5.                                              | 0004-12-27T00:00:00.000Z |
| Quarter (formatting)            | Qo           | 2019-01-01T12:13:14.015Z | 1.                                              | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | 2.                                              | 2019-04-01T00:00:00.000Z |
|                                 | QQQ          | 2019-01-01T12:13:14.015Z | 1. кв.                                          | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | 2. кв.                                          | 2019-04-01T00:00:00.000Z |
|                                 | QQQQ         | 2019-01-01T12:13:14.015Z | 1. квартал                                      | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | 2. квартал                                      | 2019-04-01T00:00:00.000Z |
|                                 | QQQQQ        | 2019-01-01T12:13:14.015Z | 1.                                              | Invalid Date             |
|                                 |              | 2019-04-01T12:13:14.015Z | 2.                                              | Invalid Date             |
| Quarter (stand-alone)           | qo           | 2019-01-01T12:13:14.015Z | 1.                                              | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | 2.                                              | 2019-04-01T00:00:00.000Z |
|                                 | qqq          | 2019-01-01T12:13:14.015Z | 1. кв.                                          | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | 2. кв.                                          | 2019-04-01T00:00:00.000Z |
|                                 | qqqq         | 2019-01-01T12:13:14.015Z | 1. квартал                                      | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | 2. квартал                                      | 2019-04-01T00:00:00.000Z |
| Month (formatting)              | Mo           | 2019-02-11T12:13:14.015Z | 2.                                              | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 7.                                              | 2019-07-01T00:00:00.000Z |
|                                 | MMM          | 2019-02-11T12:13:14.015Z | феб                                             | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | јул                                             | 2019-07-01T00:00:00.000Z |
|                                 | MMMM         | 2019-02-11T12:13:14.015Z | фебруар                                         | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | јул                                             | 2019-07-01T00:00:00.000Z |
|                                 | MMMMM        | 2019-02-11T12:13:14.015Z | 2.                                              | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 7.                                              | 2019-01-01T00:00:00.000Z |
| Month (stand-alone)             | Lo           | 2019-02-11T12:13:14.015Z | 2.                                              | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 7.                                              | 2019-07-01T00:00:00.000Z |
|                                 | LLL          | 2019-02-11T12:13:14.015Z | феб                                             | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | јул                                             | 2019-07-01T00:00:00.000Z |
|                                 | LLLL         | 2019-02-11T12:13:14.015Z | фебруар                                         | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | јул                                             | 2019-07-01T00:00:00.000Z |
|                                 | LLLLL        | 2019-02-11T12:13:14.015Z | 2.                                              | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 7.                                              | 2019-01-01T00:00:00.000Z |
| Local week of year              | wo           | 2019-01-01T12:13:14.015Z | 1.                                              | 2018-12-31T00:00:00.000Z |
|                                 |              | 2019-12-01T12:13:14.015Z | 48.                                             | 2019-11-25T00:00:00.000Z |
| ISO week of year                | Io           | 2019-01-01T12:13:14.015Z | 1.                                              | 2018-12-31T00:00:00.000Z |
|                                 |              | 2019-12-01T12:13:14.015Z | 48.                                             | 2019-11-25T00:00:00.000Z |
| Day of month                    | do           | 2019-02-11T12:13:14.015Z | 11.                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-28T12:13:14.015Z | 28.                                             | 2019-02-28T00:00:00.000Z |
| Day of year                     | Do           | 2019-02-11T12:13:14.015Z | 42.                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-12-31T12:13:14.015Z | 365.                                            | 2019-12-31T00:00:00.000Z |
| Day of week (formatting)        | E            | 2019-02-11T12:13:14.015Z | пон                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | пет                                             | 2019-02-15T00:00:00.000Z |
|                                 | EE           | 2019-02-11T12:13:14.015Z | пон                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | пет                                             | 2019-02-15T00:00:00.000Z |
|                                 | EEE          | 2019-02-11T12:13:14.015Z | пон                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | пет                                             | 2019-02-15T00:00:00.000Z |
|                                 | EEEE         | 2019-02-11T12:13:14.015Z | понедељак                                       | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | петак                                           | 2019-02-15T00:00:00.000Z |
|                                 | EEEEE        | 2019-02-11T12:13:14.015Z | П                                               | 2019-02-17T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | П                                               | 2019-02-17T00:00:00.000Z |
|                                 | EEEEEE       | 2019-02-11T12:13:14.015Z | пон                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | пет                                             | 2019-02-15T00:00:00.000Z |
| ISO day of week (formatting)    | io           | 2019-02-11T12:13:14.015Z | 1.                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 5.                                              | 2019-02-15T00:00:00.000Z |
|                                 | iii          | 2019-02-11T12:13:14.015Z | пон                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | пет                                             | 2019-02-15T00:00:00.000Z |
|                                 | iiii         | 2019-02-11T12:13:14.015Z | понедељак                                       | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | петак                                           | 2019-02-15T00:00:00.000Z |
|                                 | iiiii        | 2019-02-11T12:13:14.015Z | П                                               | 2019-02-17T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | П                                               | 2019-02-17T00:00:00.000Z |
|                                 | iiiiii       | 2019-02-11T12:13:14.015Z | пон                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | пет                                             | 2019-02-15T00:00:00.000Z |
| Local day of week (formatting)  | eo           | 2019-02-11T12:13:14.015Z | 1.                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 5.                                              | 2019-02-15T00:00:00.000Z |
|                                 | eee          | 2019-02-11T12:13:14.015Z | пон                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | пет                                             | 2019-02-15T00:00:00.000Z |
|                                 | eeee         | 2019-02-11T12:13:14.015Z | понедељак                                       | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | петак                                           | 2019-02-15T00:00:00.000Z |
|                                 | eeeee        | 2019-02-11T12:13:14.015Z | П                                               | 2019-02-17T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | П                                               | 2019-02-17T00:00:00.000Z |
|                                 | eeeeee       | 2019-02-11T12:13:14.015Z | пон                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | пет                                             | 2019-02-15T00:00:00.000Z |
| Local day of week (stand-alone) | co           | 2019-02-11T12:13:14.015Z | 1.                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 5.                                              | 2019-02-15T00:00:00.000Z |
|                                 | ccc          | 2019-02-11T12:13:14.015Z | пон                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | пет                                             | 2019-02-15T00:00:00.000Z |
|                                 | cccc         | 2019-02-11T12:13:14.015Z | понедељак                                       | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | петак                                           | 2019-02-15T00:00:00.000Z |
|                                 | ccccc        | 2019-02-11T12:13:14.015Z | П                                               | 2019-02-17T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | П                                               | 2019-02-17T00:00:00.000Z |
|                                 | cccccc       | 2019-02-11T12:13:14.015Z | пон                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | пет                                             | 2019-02-15T00:00:00.000Z |
| AM, PM                          | a            | 2019-02-11T11:13:14.015Z | АМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | ПМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | ПМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | АМ                                              | 2019-02-11T00:00:00.000Z |
|                                 | aa           | 2019-02-11T11:13:14.015Z | АМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | ПМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | ПМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | АМ                                              | 2019-02-11T00:00:00.000Z |
|                                 | aaa          | 2019-02-11T11:13:14.015Z | ам                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | пм                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | пм                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | ам                                              | 2019-02-11T00:00:00.000Z |
|                                 | aaaa         | 2019-02-11T11:13:14.015Z | AM                                              | Invalid Date             |
|                                 |              | 2019-02-11T14:13:14.015Z | PM                                              | Invalid Date             |
|                                 |              | 2019-02-11T19:13:14.015Z | PM                                              | Invalid Date             |
|                                 |              | 2019-02-11T02:13:14.015Z | AM                                              | Invalid Date             |
|                                 | aaaaa        | 2019-02-11T11:13:14.015Z | АМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | ПМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | ПМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | АМ                                              | 2019-02-11T00:00:00.000Z |
| AM, PM, noon, midnight          | b            | 2019-02-11T11:13:14.015Z | АМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | ПМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | ПМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | АМ                                              | 2019-02-11T00:00:00.000Z |
|                                 | bb           | 2019-02-11T11:13:14.015Z | АМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | ПМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | ПМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | АМ                                              | 2019-02-11T00:00:00.000Z |
|                                 | bbb          | 2019-02-11T11:13:14.015Z | ам                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | пм                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | пм                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | ам                                              | 2019-02-11T00:00:00.000Z |
|                                 | bbbb         | 2019-02-11T11:13:14.015Z | AM                                              | Invalid Date             |
|                                 |              | 2019-02-11T14:13:14.015Z | PM                                              | Invalid Date             |
|                                 |              | 2019-02-11T19:13:14.015Z | PM                                              | Invalid Date             |
|                                 |              | 2019-02-11T02:13:14.015Z | AM                                              | Invalid Date             |
|                                 | bbbbb        | 2019-02-11T11:13:14.015Z | АМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | ПМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | ПМ                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | АМ                                              | 2019-02-11T00:00:00.000Z |
| Flexible day period             | B            | 2019-02-11T11:13:14.015Z | ујутру                                          | 2019-02-11T04:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | поподне                                         | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | увече                                           | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | ноћу                                            | 2019-02-11T00:00:00.000Z |
|                                 | BB           | 2019-02-11T11:13:14.015Z | ујутру                                          | 2019-02-11T04:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | поподне                                         | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | увече                                           | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | ноћу                                            | 2019-02-11T00:00:00.000Z |
|                                 | BBB          | 2019-02-11T11:13:14.015Z | ујутру                                          | 2019-02-11T04:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | поподне                                         | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | увече                                           | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | ноћу                                            | 2019-02-11T00:00:00.000Z |
|                                 | BBBB         | 2019-02-11T11:13:14.015Z | ујутру                                          | 2019-02-11T04:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | после подне                                     | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | увече                                           | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | ноћу                                            | 2019-02-11T00:00:00.000Z |
|                                 | BBBBB        | 2019-02-11T11:13:14.015Z | ујутру                                          | 2019-02-11T04:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | поподне                                         | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | увече                                           | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | ноћу                                            | 2019-02-11T00:00:00.000Z |
| Hour [1-12]                     | ho           | 2019-02-11T11:13:14.015Z | 11.                                             | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 11.                                             | 2019-02-11T23:00:00.000Z |
| Hour [0-23]                     | Ho           | 2019-02-11T11:13:14.015Z | 11.                                             | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 23.                                             | 2019-02-11T23:00:00.000Z |
| Hour [0-11]                     | Ko           | 2019-02-11T11:13:14.015Z | 11.                                             | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 11.                                             | 2019-02-11T23:00:00.000Z |
| Hour [1-24]                     | ko           | 2019-02-11T11:13:14.015Z | 11.                                             | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 23.                                             | 2019-02-11T23:00:00.000Z |
| Minute                          | mo           | 2019-01-01T12:01:14.015Z | 1.                                              | 2019-01-01T12:01:00.000Z |
|                                 |              | 2019-04-01T12:55:14.015Z | 55.                                             | 2019-04-01T12:55:00.000Z |
| Second                          | so           | 2019-01-01T12:13:01.015Z | 1.                                              | 2019-01-01T12:13:01.000Z |
|                                 |              | 2019-04-01T12:13:55.015Z | 55.                                             | 2019-04-01T12:13:55.000Z |
| Long localized date             | P            | 1987-02-11T12:13:14.015Z | 11. 02. 87.                                     | 1987-02-11T00:00:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 29. 05. 53.                                     | 1453-05-29T00:00:00.000Z |
|                                 | PP           | 1987-02-11T12:13:14.015Z | 11. феб 87.                                     | 1987-02-11T00:00:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 29. мај 53.                                     | 1453-05-29T00:00:00.000Z |
|                                 | PPP          | 1987-02-11T12:13:14.015Z | 11. фебруар 1987.                               | 1987-02-11T00:00:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 29. мај 1453.                                   | 1453-05-29T00:00:00.000Z |
|                                 | PPPP         | 1987-02-11T12:13:14.015Z | среда, 11. фебруар 1987.                        | 1987-02-11T00:00:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | недеља, 29. мај 1453.                           | 1453-05-29T00:00:00.000Z |
| Long localized time             | p            | 1987-02-11T12:13:14.015Z | 12:13                                           | 1987-02-11T12:13:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 23:59                                           | 1453-05-29T23:59:00.000Z |
|                                 | pp           | 1987-02-11T12:13:14.015Z | 12:13:14                                        | 1987-02-11T12:13:14.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 23:59:59                                        | 1453-05-29T23:59:59.000Z |
|                                 | ppp          | 1987-02-11T12:13:14.015Z | 12:13:14 GMT+0                                  | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | 23:59:59 GMT+0                                  | Errored                  |
|                                 | pppp         | 1987-02-11T12:13:14.015Z | 12:13:14 (GMT+00:00)                            | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | 23:59:59 (GMT+00:00)                            | Errored                  |
| Combination of date and time    | Pp           | 1987-02-11T12:13:14.015Z | 11. 02. 87. 12:13                               | 1987-02-11T12:13:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 29. 05. 53. 23:59                               | 1453-05-29T23:59:00.000Z |
|                                 | PPpp         | 1987-02-11T12:13:14.015Z | 11. феб 87. 12:13:14                            | 1987-02-11T12:13:14.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 29. мај 53. 23:59:59                            | 1453-05-29T23:59:59.000Z |
|                                 | PPPppp       | 1987-02-11T12:13:14.015Z | 11. фебруар 1987. у 12:13:14 GMT+0              | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | 29. мај 1453. у 23:59:59 GMT+0                  | Errored                  |
|                                 | PPPPpppp     | 1987-02-11T12:13:14.015Z | среда, 11. фебруар 1987. у 12:13:14 (GMT+00:00) | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | недеља, 29. мај 1453. у 23:59:59 (GMT+00:00)    | Errored                  |

## `formatDistance`

If now is January 1st, 2000, 00:00.

| Date                     | Result           | `includeSeconds: true` | `addSuffix: true`    |
| ------------------------ | ---------------- | ---------------------- | -------------------- |
| 2006-01-01T00:00:00.000Z | око 6 година     | око 6 година           | за око 6 година      |
| 2005-01-01T00:00:00.000Z | око 5 година     | око 5 година           | за око 5 година      |
| 2004-01-01T00:00:00.000Z | око 4 године     | око 4 године           | за око 4 године      |
| 2003-01-01T00:00:00.000Z | око 3 године     | око 3 године           | за око 3 године      |
| 2002-01-01T00:00:00.000Z | око 2 године     | око 2 године           | за око 2 године      |
| 2001-06-01T00:00:00.000Z | преко 1 годину   | преко 1 годину         | за преко 1 годину    |
| 2001-02-01T00:00:00.000Z | око 1 годину     | око 1 годину           | за око 1 годину      |
| 2001-01-01T00:00:00.000Z | око 1 годину     | око 1 годину           | за око 1 годину      |
| 2000-06-01T00:00:00.000Z | 5 месеци         | 5 месеци               | за 5 месеци          |
| 2000-03-01T00:00:00.000Z | 2 месеца         | 2 месеца               | за 2 месеца          |
| 2000-02-01T00:00:00.000Z | око 1 месец      | око 1 месец            | за око 1 месец       |
| 2000-01-15T00:00:00.000Z | 14 дана          | 14 дана                | за 14 дана           |
| 2000-01-02T00:00:00.000Z | 1 дан            | 1 дан                  | за 1 дан             |
| 2000-01-01T06:00:00.000Z | око 6 сати       | око 6 сати             | за око 6 сати        |
| 2000-01-01T01:00:00.000Z | око 1 сат        | око 1 сат              | за око 1 сат         |
| 2000-01-01T00:45:00.000Z | око 1 сат        | око 1 сат              | за око 1 сат         |
| 2000-01-01T00:30:00.000Z | 30 минута        | 30 минута              | за 30 минута         |
| 2000-01-01T00:15:00.000Z | 15 минута        | 15 минута              | за 15 минута         |
| 2000-01-01T00:01:00.000Z | 1 минута         | 1 минута               | за 1 минуту          |
| 2000-01-01T00:00:25.000Z | мање од 1 минуте | пола минуте            | за мање од 1 минуту  |
| 2000-01-01T00:00:15.000Z | мање од 1 минуте | мање од 20 секунди     | за мање од 1 минуту  |
| 2000-01-01T00:00:05.000Z | мање од 1 минуте | мање од 10 секунди     | за мање од 1 минуту  |
| 2000-01-01T00:00:00.000Z | мање од 1 минуте | мање од 5 секунди      | пре мање од 1 минуте |
| 1999-12-31T23:59:55.000Z | мање од 1 минуте | мање од 10 секунди     | пре мање од 1 минуте |
| 1999-12-31T23:59:45.000Z | мање од 1 минуте | мање од 20 секунди     | пре мање од 1 минуте |
| 1999-12-31T23:59:35.000Z | мање од 1 минуте | пола минуте            | пре мање од 1 минуте |
| 1999-12-31T23:59:00.000Z | 1 минута         | 1 минута               | пре 1 минуте         |
| 1999-12-31T23:45:00.000Z | 15 минута        | 15 минута              | пре 15 минута        |
| 1999-12-31T23:30:00.000Z | 30 минута        | 30 минута              | пре 30 минута        |
| 1999-12-31T23:15:00.000Z | око 1 сат        | око 1 сат              | пре око 1 сат        |
| 1999-12-31T23:00:00.000Z | око 1 сат        | око 1 сат              | пре око 1 сат        |
| 1999-12-31T18:00:00.000Z | око 6 сати       | око 6 сати             | пре око 6 сати       |
| 1999-12-30T00:00:00.000Z | 2 дана           | 2 дана                 | пре 2 дана           |
| 1999-12-15T00:00:00.000Z | 17 дана          | 17 дана                | пре 17 дана          |
| 1999-12-01T00:00:00.000Z | око 1 месец      | око 1 месец            | пре око 1 месец      |
| 1999-11-01T00:00:00.000Z | 2 месеца         | 2 месеца               | пре 2 месеца         |
| 1999-06-01T00:00:00.000Z | 7 месеци         | 7 месеци               | пре 7 месеци         |
| 1999-01-01T00:00:00.000Z | око 1 годину     | око 1 годину           | пре око 1 годину     |
| 1998-12-01T00:00:00.000Z | око 1 годину     | око 1 годину           | пре око 1 годину     |
| 1998-06-01T00:00:00.000Z | преко 1 годину   | преко 1 годину         | пре преко 1 годину   |
| 1998-01-01T00:00:00.000Z | око 2 године     | око 2 године           | пре око 2 године     |
| 1997-01-01T00:00:00.000Z | око 3 године     | око 3 године           | пре око 3 године     |
| 1996-01-01T00:00:00.000Z | око 4 године     | око 4 године           | пре око 4 године     |
| 1995-01-01T00:00:00.000Z | око 5 година     | око 5 година           | пре око 5 година     |
| 1994-01-01T00:00:00.000Z | око 6 година     | око 6 година           | пре око 6 година     |

## `formatDistanceStrict`

If now is January 1st, 2000, 00:00.

| Date                     | Result     | `addSuffix: true` | With forced unit (i.e. `hour`) |
| ------------------------ | ---------- | ----------------- | ------------------------------ |
| 2006-01-01T00:00:00.000Z | 6 година   | за 6 година       | 52608 сати                     |
| 2005-01-01T00:00:00.000Z | 5 година   | за 5 година       | 43848 сати                     |
| 2004-01-01T00:00:00.000Z | 4 године   | за 4 године       | 35064 сата                     |
| 2003-01-01T00:00:00.000Z | 3 године   | за 3 године       | 26304 сата                     |
| 2002-01-01T00:00:00.000Z | 2 године   | за 2 године       | 17544 сата                     |
| 2001-06-01T00:00:00.000Z | 1 година   | за 1 годину       | 12408 сати                     |
| 2001-02-01T00:00:00.000Z | 1 година   | за 1 годину       | 9528 сати                      |
| 2001-01-01T00:00:00.000Z | 1 година   | за 1 годину       | 8784 сата                      |
| 2000-06-01T00:00:00.000Z | 5 месеци   | за 5 месеци       | 3648 сати                      |
| 2000-03-01T00:00:00.000Z | 2 месеца   | за 2 месеца       | 1440 сати                      |
| 2000-02-01T00:00:00.000Z | 1 месец    | за 1 месец        | 744 сата                       |
| 2000-01-15T00:00:00.000Z | 14 дана    | за 14 дана        | 336 сати                       |
| 2000-01-02T00:00:00.000Z | 1 дан      | за 1 дан          | 24 сата                        |
| 2000-01-01T06:00:00.000Z | 6 сати     | за 6 сати         | 6 сати                         |
| 2000-01-01T01:00:00.000Z | 1 сат      | за 1 сат          | 1 сат                          |
| 2000-01-01T00:45:00.000Z | 45 минута  | за 45 минута      | 1 сат                          |
| 2000-01-01T00:30:00.000Z | 30 минута  | за 30 минута      | 1 сат                          |
| 2000-01-01T00:15:00.000Z | 15 минута  | за 15 минута      | 0 сати                         |
| 2000-01-01T00:01:00.000Z | 1 минута   | за 1 минуту       | 0 сати                         |
| 2000-01-01T00:00:25.000Z | 25 секунди | за 25 секунди     | 0 сати                         |
| 2000-01-01T00:00:15.000Z | 15 секунди | за 15 секунди     | 0 сати                         |
| 2000-01-01T00:00:05.000Z | 5 секунди  | за 5 секунди      | 0 сати                         |
| 2000-01-01T00:00:00.000Z | 0 секунди  | пре 0 секунди     | 0 сати                         |
| 1999-12-31T23:59:55.000Z | 5 секунди  | пре 5 секунди     | 0 сати                         |
| 1999-12-31T23:59:45.000Z | 15 секунди | пре 15 секунди    | 0 сати                         |
| 1999-12-31T23:59:35.000Z | 25 секунди | пре 25 секунди    | 0 сати                         |
| 1999-12-31T23:59:00.000Z | 1 минута   | пре 1 минуте      | 0 сати                         |
| 1999-12-31T23:45:00.000Z | 15 минута  | пре 15 минута     | 0 сати                         |
| 1999-12-31T23:30:00.000Z | 30 минута  | пре 30 минута     | 1 сат                          |
| 1999-12-31T23:15:00.000Z | 45 минута  | пре 45 минута     | 1 сат                          |
| 1999-12-31T23:00:00.000Z | 1 сат      | пре 1 сат         | 1 сат                          |
| 1999-12-31T18:00:00.000Z | 6 сати     | пре 6 сати        | 6 сати                         |
| 1999-12-30T00:00:00.000Z | 2 дана     | пре 2 дана        | 48 сати                        |
| 1999-12-15T00:00:00.000Z | 17 дана    | пре 17 дана       | 408 сати                       |
| 1999-12-01T00:00:00.000Z | 1 месец    | пре 1 месец       | 744 сата                       |
| 1999-11-01T00:00:00.000Z | 2 месеца   | пре 2 месеца      | 1464 сата                      |
| 1999-06-01T00:00:00.000Z | 7 месеци   | пре 7 месеци      | 5136 сати                      |
| 1999-01-01T00:00:00.000Z | 1 година   | пре 1 године      | 8760 сати                      |
| 1998-12-01T00:00:00.000Z | 1 година   | пре 1 године      | 9504 сата                      |
| 1998-06-01T00:00:00.000Z | 2 године   | пре 2 године      | 13896 сати                     |
| 1998-01-01T00:00:00.000Z | 2 године   | пре 2 године      | 17520 сати                     |
| 1997-01-01T00:00:00.000Z | 3 године   | пре 3 године      | 26280 сати                     |
| 1996-01-01T00:00:00.000Z | 4 године   | пре 4 године      | 35064 сата                     |
| 1995-01-01T00:00:00.000Z | 5 година   | пре 5 година      | 43824 сата                     |
| 1994-01-01T00:00:00.000Z | 6 година   | пре 6 година      | 52584 сата                     |

## `formatRelative`

If now is January 1st, 2000, 00:00.

| Date                     | Result                   |
| ------------------------ | ------------------------ |
| 2000-01-10T00:00:00.000Z | 10. 01. 00.              |
| 2000-01-05T00:00:00.000Z | следећу среду у 00:00    |
| 2000-01-02T00:00:00.000Z | сутра у 00:00            |
| 2000-01-01T00:00:00.000Z | данас у 00:00            |
| 1999-12-31T00:00:00.000Z | јуче у 00:00             |
| 1999-12-27T00:00:00.000Z | прошли понедељак у 00:00 |
| 1999-12-21T00:00:00.000Z | 21. 12. 99.              |

## `formatDuration`

| Duration      | Result    |
| ------------- | --------- |
| {"years":0}   | 0 година  |
| {"years":1}   | 1 година  |
| {"years":2}   | 2 године  |
| {"months":0}  | 0 месеци  |
| {"months":1}  | 1 месец   |
| {"months":2}  | 2 месеца  |
| {"weeks":0}   | 0 недеље  |
| {"weeks":1}   | 1 недељу  |
| {"weeks":2}   | 2 недеље  |
| {"days":0}    | 0 дана    |
| {"days":1}    | 1 дан     |
| {"days":2}    | 2 дана    |
| {"hours":0}   | 0 сати    |
| {"hours":1}   | 1 сат     |
| {"hours":2}   | 2 сата    |
| {"minutes":0} | 0 минута  |
| {"minutes":1} | 1 минута  |
| {"minutes":2} | 2 минуте  |
| {"seconds":0} | 0 секунди |
| {"seconds":1} | 1 секунда |
| {"seconds":2} | 2 секунде |