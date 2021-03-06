> npm install -g hacker-job-trends

## hacker-job-trends

As we know, an "Ask HN: Who is Hiring?"([example](https://news.ycombinator.com/item?id=17442187)) post will occur at hackernews every month. It is interesting to scan the post because it helps you to get a feeling about what is happening in tec related business. This repo aims to help you keep up with how the tec job requirements/used tools/kind/... evolve.

## How

1.  Get historical "Who is hiring" posts on HackerNews
2.  Analyes the keyword count history

## Examples

#### remote job trends:

```bash
$ hjt 'remote' - 'not remote' - 'no remote'

 123.00 ┤                                                                                         ╭
 115.53 ┤                                                                                         │
 108.07 ┤                                                                             ╭╮          │
 100.60 ┤                                                                             ││    ╭╮ ╭╮╭╯
  93.13 ┤                                                                            ╭╯╰╮   ││ │││
  85.67 ┤                                       ╭╮                                   │  ╰╮  ││ │╰╯
  78.20 ┤                                       ││                  ╭╮   ╭╮       ╭╮ │   │ ╭╯╰─╯
  70.73 ┤                                       ││  ╭╮ ╭╮ ╭╮   ╭╮  ╭╯╰─╮ │╰──╮ ╭╮╭╯│╭╯   │ │
  63.27 ┤                        ╭╮         ╭─╮ ││ ╭╯╰╮│╰─╯╰╮╭╮│╰──╯   │╭╯   ╰─╯╰╯ ││    ╰╮│
  55.80 ┤   ╭╮                 ╭╮││╭╮ ╭╮╭╮  │ ╰─╯╰─╯  ││    ││││       ╰╯          ╰╯     ││
  48.33 ┤   │╰╮      ╭──╮      │││││╰╮│╰╯│  │         ╰╯    ╰╯╰╯                          ╰╯
  40.87 ┤╭╮ │ ╰╮╭╮  ╭╯  ╰─╮╭╮╭─╯╰╯╰╯ ╰╯  ╰──╯
  33.40 ┤││ │  ╰╯╰╮╭╯     ││╰╯
  25.93 ┤││╭╯     ╰╯      ╰╯
  18.47 ┼╯││
  11.00 ┤ ╰╯
        :
        ┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──
      2011-01     2012-01     2013-01     2014-01     2015-01     2016-01     2017-01     2018-01     2019-01
```

#### blockchain trends

```
$ hjt 'ethereum' + 'blockchain' + 'bitcoin' + 'solidity' + 'smart contract'

  40.00 ┼                                                                                         ╭ 
  37.33 ┤                                                                                         │ 
  34.67 ┤                                                                                 ╭╮      │ 
  32.00 ┤                                                                                 ││      │ 
  29.33 ┤                                                                                ╭╯╰─╮   ╭╯ 
  26.67 ┤                                                                                │   │   │  
  24.00 ┤                                                                                │   │   │  
  21.33 ┤                                                                               ╭╯   │   │  
  18.67 ┤                                                                               │    │   │  
  16.00 ┤                                                                         ╭╮    │    │   │  
  13.33 ┤                                                                    ╭╮   ││    │    │  ╭╯  
  10.67 ┤                                                  ╭╮                ││   ││    │    ╰──╯   
   8.00 ┤                                                  ││              ╭╮││   ││    │           
   5.33 ┤                               ╭╮  ╭╮    ╭╮       │╰╮        ╭╮   ││││ ╭╮││╭╮  │           
   2.67 ┤                              ╭╯╰╮ │╰─╮ ╭╯╰─────╮ │ │  ╭──╮  │╰╮╭╮││││ │││╰╯│╭─╯           
   0.00 ┼──────────────────────────────╯  ╰─╯  ╰─╯       ╰─╯ ╰──╯  ╰──╯ ╰╯╰╯╰╯╰─╯╰╯  ╰╯             
        :
        ┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──
       2011-01     2012-01     2013-01     2014-01     2015-01     2016-01     2017-01     2018-01     2019-01

```

#### java trends:

```bash
$ hjt 'java' - 'javascript'

  66.00 ┤            ╭╮
  61.87 ┤            ││
  57.73 ┤            ││      ╭╮
  53.60 ┤            ││      ││
  49.47 ┤            ││      ││  ╭╮       ╭╮
  45.33 ┤            ││╭╮    ││  ││    ╭╮ ││         ╭╮     ╭╮
  41.20 ┤          ╭╮││││    ││ ╭╯│    ││ ││     ╭╮  ││     ││
  37.07 ┤   ╭╮  ╭╮╭╯│││││    ││╭╯ │╭╮╭╮││ ││     │╰──╯│╭╮ ╭╮││
  32.93 ┤  ╭╯│╭╮│││ ││╰╯╰╮╭╮╭╯╰╯  │││││││ │╰╮╭╮  │    ╰╯│ ││││     ╭╮                             ╭
  28.80 ┤  │ ││││╰╯ ││   ╰╯╰╯     ╰╯╰╯╰╯╰─╯ │││ ╭╯      ╰╮│││╰╮╭╮╭─╯│      ╭╮                   ╭╮│
  24.67 ┤╭╮│ ╰╯╰╯   ╰╯                      │││╭╯        ││││ ││╰╯  │ ╭─╮  ││              ╭╮╭╮ │││
  20.53 ┤│││                                ╰╯╰╯         ││││ ││    │╭╯ │ ╭╯│    ╭╮  ╭╮    ││││ │╰╯
  16.40 ┤│││                                             ╰╯╰╯ ╰╯    ││  ╰─╯ ╰╮╭─╮││ ╭╯╰╮ ╭╮││││╭╯
  12.27 ┼╯││                                                        ╰╯       ╰╯ ││╰╮│  ╰─╯╰╯╰╯╰╯
   8.13 ┤ ╰╯                                                                    ││ ╰╯
   4.00 ┤                                                                       ╰╯
        :
        ┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──
       2011-01     2012-01     2013-01     2014-01     2015-01     2016-01     2017-01     2018-01     2019-01
```

#### javascript trends:

```bash
$ hjt 'javascript' + ' js '

  97.00 ┼                                           ╭╮
  90.73 ┤                                           ││
  84.47 ┤                                   ╭╮      ││
  78.20 ┤                 ╭─╮       ╭╮      │╰╮     ││
  71.93 ┤              ╭╮ │ │╭╮ ╭──╮││ ╭╮ ╭╮│ │     │╰╮╭╮
  65.67 ┤     ╭╮      ╭╯│ │ │││╭╯  │││╭╯│ │││ │  ╭╮╭╯ ╰╯╰╮
  59.40 ┤     ││╭╮   ╭╯ │╭╯ ╰╯╰╯   ││╰╯ │ │╰╯ │  │╰╯     │       ╭╮ ╭╮
  53.13 ┤  ╭╮╭╯╰╯│ ╭╮│  ╰╯         ╰╯   │╭╯   ╰╮╭╯       │  ╭╮   │╰─╯╰╮   ╭╮╭╮
  46.87 ┤  │╰╯   │╭╯││                  ╰╯     ╰╯        ╰╮ ││   │    ╰─╮ │╰╯╰─╮    ╭╮      ╭╮  ╭╮╭
  40.60 ┤  │     ││ ╰╯                                    │ ││ ╭─╯      │ │    │ ╭╮ │╰╮╭─╮ ╭╯│ ╭╯╰╯
  34.33 ┤  │     ╰╯                                       ╰╮│╰─╯        │ │    │ │╰╮│ ││ ╰╮│ ╰─╯
  28.07 ┤╭╮│                                               ╰╯           ╰─╯    │ │ ││ ╰╯  ╰╯
  21.80 ┤│││                                                                   ╰╮│ ││
  15.53 ┼╯││                                                                    ╰╯ ╰╯
   9.27 ┤ ││
   3.00 ┤ ╰╯
        :
        ┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──
      2011-01     2012-01     2013-01     2014-01     2015-01     2016-01     2017-01     2018-01     2019-01
```

### nodejs trends

```bash
$ hjt 'nodejs' + 'node.js'

  30.00 ┼                                          ╭╮            ╭╮
  28.00 ┤                                          │╰╮           ││
  26.00 ┤                                          │ │   ╭╮      ││
  24.00 ┤                                          │ │╭╮╭╯│      ││                               ╭
  22.00 ┤                      ╭╮      ╭╮    ╭╮ ╭──╯ ││╰╯ ╰╮     ││                             ╭╮│
  20.00 ┤                      ││      ││    │╰╮│    ╰╯    │     ││╭╮                       ╭╮  │││
  18.00 ┤         ╭─╮╭─╮       ││      ││ ╭╮ │ ││          │    ╭╯│││         ╭╮            ││  │││
  16.00 ┤      ╭╮ │ ││ ╰─╮ ╭╮ ╭╯│╭╮    ││╭╯╰╮│ ╰╯          │   ╭╯ │││     ╭╮ ╭╯│ ╭╮    ╭╮   ││  │╰╯
  14.00 ┤      │╰╮│ ╰╯   │ ││╭╯ ││╰─╮  │││  ││             │╭──╯  ╰╯│ ╭╮ ╭╯│╭╯ │ │╰╮ ╭╮│╰╮  ││  │
  12.00 ┤     ╭╯ ╰╯      ╰─╯╰╯  ││  ╰╮╭╯││  ││             ││       │╭╯╰╮│ ╰╯  │ │ │ │╰╯ │  ││  │
  10.00 ┤  ╭╮╭╯                 ╰╯   ╰╯ ╰╯  ╰╯             ╰╯       ╰╯  ││     ╰╮│ │╭╯   ╰╮ │╰╮ │
   8.00 ┤  │╰╯                                                          ╰╯      ╰╯ ││     ╰─╯ │╭╯
   6.00 ┤╭╮│                                                                       ╰╯         ╰╯
   4.00 ┤│││
   2.00 ┤│╰╯
   0.00 ┼╯
        :
        ┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──
      2011-01     2012-01     2013-01     2014-01     2015-01     2016-01     2017-01     2018-01     2019-01
```

#### react trends

```bash
$ hjt react

  97.00 ┼                                                                                        ╭─
  90.53 ┤                                                                                        │
  84.07 ┤                                                                                        │
  77.60 ┤                                                                                       ╭╯
  71.13 ┤                                                                                       │
  64.67 ┤                                                                     ╭╮    ╭╮        ╭╮│
  58.20 ┤                                                                     ││ ╭╮ ││╭─╮╭╮ ╭╮│╰╯
  51.73 ┤                                                                 ╭╮ ╭╯╰╮││ │││ ╰╯╰╮│││
  45.27 ┤                                                             ╭╮  ││╭╯  │││ │││    ╰╯╰╯
  38.80 ┤                                                        ╭╮╭─╮││ ╭╯╰╯   │││ │╰╯
  32.33 ┤                                                        │╰╯ ╰╯╰─╯      ││╰╮│
  25.87 ┤                                                   ╭─╮╭╮│              ││ ╰╯
  19.40 ┤                                                   │ ╰╯╰╯              ╰╯
  12.93 ┤                                          ╭╮ ╭╮  ╭─╯
   6.47 ┤                                    ╭╮╭───╯╰─╯╰──╯
   0.00 ┼────────────────────────────────────╯╰╯
        :
        ┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──
       2011-01     2012-01     2013-01     2014-01     2015-01     2016-01     2017-01     2018-01     2019-01
```

#### python trends

```bash
$ hjt python

  83.00 ┼                                    ╭╮    ╭──╮
  77.60 ┤                ╭╮   ╭─╮      ╭╮    ││    │  │     ╭╮                                    ╭
  72.20 ┤                ││╭╮╭╯ │      ││    ││    │  ╰╮    ││   ╭╮                               │
  66.80 ┤       ╭╮      ╭╯││││  ╰─╮    ││╭╮  │╰╮╭╮╭╯   ╰─╮  ││   ││ ╭╮╭╮                         ╭╯
  61.40 ┤       ││   ╭─╮│ ││││    │╭╮  │││╰╮ │ ││╰╯      │  ││ ╭─╯│ │╰╯│   ╭╮         ╭╮       ╭╮│
  56.00 ┤       ││ ╭╮│ ││ ││││    │││  │││ │╭╯ ││        ╰╮ ││ │  │╭╯  ╰╮ ╭╯│  ╭╮     ││╭╮     │││
  50.60 ┤  ╭╮   ││ │││ ││ ╰╯╰╯    ││╰──╯││ ╰╯  ││         ╰─╯╰─╯  ││    │╭╯ ╰──╯╰───╮ │││╰╮ ╭╮ │││
  45.20 ┤  │╰╮╭╮││ │││ ╰╯         ╰╯    ╰╯     ││                 ││    ││          ╰─╯╰╯ │ ││ │╰╯
  39.80 ┤  │ ││╰╯│ │││                         ││                 ││    ││                ╰─╯│ │
  34.40 ┤  │ ╰╯  ╰─╯││                         ╰╯                 ╰╯    ││                   ╰─╯
  29.00 ┤╭╮│        ╰╯                                                  ╰╯
  23.60 ┼╯││
  18.20 ┤ ││
  12.80 ┤ ││
   7.40 ┤ ││
   2.00 ┤ ╰╯
        :
        ┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──
       2011-01     2012-01     2013-01     2014-01     2015-01     2016-01     2017-01     2018-01     2019-01
```

#### golang trends

```bash
$ hjt golang
  11.00 ┼                                                                ╭╮╭╮
  10.27 ┤                                                                │││╰─╮     ╭╮           ╭╮
   9.53 ┤                                                                │││  │     ││           ││
   8.80 ┤                                                          ╭╮    │││  │     ││           ││
   8.07 ┤                                                          ││   ╭╯││  │     ││         ╭╮││
   7.33 ┤                                     ╭╮                 ╭╮│╰─╮ │ ╰╯  │ ╭╮ ╭╯│ ╭╮   ╭╮ │╰╯╰
   6.60 ┤                                     ││                 │││  │ │     │ ││ │ │ ││   ││ │
   5.87 ┤                                     ││                 │││  │ │     ╰╮│╰╮│ │ ││  ╭╯╰╮│
   5.13 ┤                                     ││╭╮               │╰╯  ╰─╯      ╰╯ ││ │╭╯│  │  ╰╯
   4.40 ┤                                     ││││               │                ││ ││ │  │
   3.67 ┤                                     ││││╭╮       ╭╮    │                ││ ││ │  │
   2.93 ┤                                     ││││││ ╭╮ ╭╮ ││  ╭╮│                ││ ╰╯ │  │
   2.20 ┤                                     │││││╰─╯╰─╯│╭╯│╭╮│╰╯                ╰╯    ╰─╮│
   1.47 ┤                                     │││││      ││ ││││                          ││
   0.73 ┤               ╭╮             ╭╮ ╭╮ ╭╯╰╯╰╯      ││ ││╰╯                          ╰╯
   0.00 ┼───────────────╯╰─────────────╯╰─╯╰─╯           ╰╯ ╰╯
        :
        ┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──────────┼┼──
       2011-01     2012-01     2013-01     2014-01     2015-01     2016-01     2017-01     2018-01     2019-01
```

## npm package

```bash
# install package (node version > 10.0.0)
npm install -g hacker-job-trends

# see match count history on hackernews who is hiring post
hjt 'python'

# match multiple keyword and a count them together
hjt ' js ' + 'javascript'

# match multiple keywords but you want to do a subtraction operation
hjt 'remote' - 'no remote' - 'not remote'
```

## Contributing

### 1. Add new useful trend graph

By install the npm module and generate new interesting chart and open a PR for the `README.md`

### 2. Add new who is hiring link

1.  Fork the repo and `npm install`
2.  Add new "who is hiring" post url on [HN-who-is-hiring-monthly.md](./HN-who-is-hiring-monthly.md)
3.  `npm run updateContents` and make a PR

## Best search pattern for searching monthly "who is hiring" on hackernews

```bash
# Google:
Ask HN: Who is Hiring? "November 2011" site:https://news.ycombinator.com/
```
