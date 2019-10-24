# Pars Exchange API

Table of Contents :

  - [General API Information](#general-api-information)
- [Public API](#public-api)
  - [Trades](#trades)
  - [OrderBook](#orderbook)
  - [Tickers](#tickers)

## General API Information
* The base endpoint is: **https://parsxc.com/api**

## Public API

## Trades
**Url :**
https://parsxc.com/api/exchange/lasttrades/market/

**Example :**
https://parsxc.com/api/exchange/lasttrades/market/eth_btc/limit/100

```
GET /api/exchange/lasttrades/market/eth_btc/limit/100
```

**Response:**
```javascript
{
    "status": 1,
    "data": {
        "tradelog": [
            {
                "addtime": "10-16 05:55:02",
                "type": "1",
                "price": 0.022024,
                "num": "1.000000",
                "mum": "0.02"
            }
        ]
    }
}
```

## OrderBook
**Url :**
https://parsxc.com/api/exchange/activeorders/market/

**Example :**
https://parsxc.com/api/exchange/activeorders/market/eth_btc

```
GET /api/exchange/activeorders/market/eth_btc
```

**Response:**
```javascript
{
    "status": 1,
    "data": {
        "depth": {
            "buy": [
                {
                    "price": "0.01916000",
                    "nums": "0.01000000"
                },
                {
                    "price": "0.01903000",
                    "nums": "0.01580000"
                },
                {
                    "price": "0.01900100",
                    "nums": "0.00670000"
                }
            ],
            "sell": [
                {
                    "price": "0.02279000",
                    "nums": "0.04800000"
                },
                {
                    "price": "0.02285000",
                    "nums": "0.06700000"
                },
                {
                    "price": "0.02290000",
                    "nums": "0.00500000"
                },
                {
                    "price": "0.02299000",
                    "nums": "0.08561500"
                },
                {
                    "price": "0.02300000",
                    "nums": "0.10000000"
                }
            ]
        }
    }
}
```

## Tickers
**Url :**
https://parsxc.com/Api/Index/marketInfo

**Example :**
https://parsxc.com/Api/Index/marketInfo

```
GET /api/index/marketInfo
```

**Response:**
```javascript
{
    "status": 1,
    "data": {
        "market": [
            {
                "id": "17",
                "ticker": "eth_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Ethereum(ETH/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5da2c8b1246ba.png",
                "new_price": 0.022024,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.022024,
                "max_price": 0.022024,
                "change": 0,
                "volume": 1
            },
            {
                "id": "18",
                "ticker": "pars_btc",
                "fee_buy": "0.05",
                "fee_sell": "0.05",
                "name": "ParsiCoin(PARS/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5da42d4dd5bff.png",
                "new_price": 0.00000097,
                "buy_price": 0,
                "sell_price": 0.00000099,
                "min_price": 0.00000097,
                "max_price": 0.00000097,
                "change": 0,
                "volume": 1000
            },
            {
                "id": "19",
                "ticker": "pars_eth",
                "fee_buy": "0.05",
                "fee_sell": "0.05",
                "name": "ParsiCoin(PARS/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5da42d4dd5bff.png",
                "new_price": 0.000046,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.000046,
                "max_price": 0.000046,
                "change": 0,
                "volume": 0
            },
            {
                "id": "20",
                "ticker": "ltc_pars",
                "fee_buy": "0.05",
                "fee_sell": "0.05",
                "name": "Litecoin(LTC/PARS)",
                "icon": "http://parsxc.com/Upload/coin/5d8867471450b.png",
                "new_price": 8000,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 8000,
                "max_price": 8000,
                "change": 0,
                "volume": 0.02
            },
            {
                "id": "21",
                "ticker": "ltc_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Litecoin(LTC/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5d8867471450b.png",
                "new_price": 0.00671228,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.00671228,
                "max_price": 0.00671228,
                "change": -0.13,
                "volume": 0.02
            },
            {
                "id": "22",
                "ticker": "ltc_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Litecoin(LTC/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5d8867471450b.png",
                "new_price": 0.311,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.311,
                "max_price": 0.311,
                "change": 0,
                "volume": 0.03
            },
            {
                "id": "23",
                "ticker": "waves_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Waves(WAVES/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5d8c9d9cc5f5e.png",
                "new_price": 0.000095,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.000095,
                "max_price": 0.000095,
                "change": 0,
                "volume": 2
            },
            {
                "id": "24",
                "ticker": "bch_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Bitcoin Cash(BCH/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5d8c9e2ca570d.png",
                "new_price": 0.02902988,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.02902988,
                "max_price": 0.02902988,
                "change": 6.22,
                "volume": 0.012
            },
            {
                "id": "95",
                "ticker": "nmc_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Namecoin(NMC/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5da56b968529d.png",
                "new_price": 0.000057,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.000057,
                "max_price": 0.000057,
                "change": 0.25,
                "volume": 2
            },
            {
                "id": "28",
                "ticker": "dash_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Dash(DASH/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5d8c9f76d8a86.png",
                "new_price": 0.00849095,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.00849095,
                "max_price": 0.00849095,
                "change": -2.86,
                "volume": 0.02
            },
            {
                "id": "30",
                "ticker": "doge_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Dogecoin(DOGE/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5d8ca5867afc2.png",
                "new_price": 0.00000034,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.00000034,
                "max_price": 0.00000034,
                "change": 13.33,
                "volume": 25
            },
            {
                "id": "33",
                "ticker": "rvn_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Ravencoin(RVN/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5d8ca7f2e7fd5.png",
                "new_price": 0.0000038,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.0000038,
                "max_price": 0.0000038,
                "change": -8.29,
                "volume": 5
            },
            {
                "id": "35",
                "ticker": "pivx_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Pivx(PIVX/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5d8ca8b7f0694.png",
                "new_price": 0.000028,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.000028,
                "max_price": 0.000028,
                "change": -9.36,
                "volume": 6.5
            },
            {
                "id": "37",
                "ticker": "mona_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Monacoin(MONA/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5d8ca9378c2df.png",
                "new_price": 0.00013941,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.00013941,
                "max_price": 0.00013941,
                "change": 2.73,
                "volume": 5
            },
            {
                "id": "56",
                "ticker": "bch_pars",
                "fee_buy": "0.05",
                "fee_sell": "0.05",
                "name": "Bitcoin Cash(BCH/PARS)",
                "icon": "http://parsxc.com/Upload/coin/5d8c9e2ca570d.png",
                "new_price": 200000,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 200000,
                "max_price": 200000,
                "change": 0,
                "volume": 0.01
            },
            {
                "id": "39",
                "ticker": "waves_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Waves(WAVES/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5d8c9d9cc5f5e.png",
                "new_price": 0.0044,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.0044,
                "max_price": 0.0044,
                "change": 0,
                "volume": 4
            },
            {
                "id": "40",
                "ticker": "bch_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Bitcoin Cash(BCH/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5d8c9e2ca570d.png",
                "new_price": 1.333,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 1.333,
                "max_price": 1.333,
                "change": 0,
                "volume": 0.013
            },
            {
                "id": "97",
                "ticker": "nmc_usdt",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Namecoin(NMC/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5da56b968529d.png",
                "new_price": 0.4254,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.4254,
                "max_price": 0.4254,
                "change": 0,
                "volume": 4
            },
            {
                "id": "44",
                "ticker": "dash_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Dash(DASH/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5d8c9f76d8a86.png",
                "new_price": 0.39,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.39,
                "max_price": 0.39,
                "change": 0,
                "volume": 0.04
            },
            {
                "id": "46",
                "ticker": "doge_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Dogecoin(DOGE/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5d8ca5867afc2.png",
                "new_price": 0.000016,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.000016,
                "max_price": 0.000016,
                "change": 0,
                "volume": 40
            },
            {
                "id": "49",
                "ticker": "rvn_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Ravencoin(RVN/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5d8ca7f2e7fd5.png",
                "new_price": 0.00017,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.00017,
                "max_price": 0.00017,
                "change": 0,
                "volume": 6
            },
            {
                "id": "51",
                "ticker": "pivx_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Pivx(PIVX/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5d8ca8b7f0694.png",
                "new_price": 0.0013,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.0013,
                "max_price": 0.0013,
                "change": 0,
                "volume": 4.5
            },
            {
                "id": "53",
                "ticker": "mona_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Monacoin(MONA/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5d8ca9378c2df.png",
                "new_price": 0.0064,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.0064,
                "max_price": 0.0064,
                "change": 0,
                "volume": 1
            },
            {
                "id": "92",
                "ticker": "xvg_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Verge(XVG/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5d8d26b41eebc.png",
                "new_price": 0.00000042,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.00000042,
                "max_price": 0.00000042,
                "change": -6.67,
                "volume": 4
            },
            {
                "id": "96",
                "ticker": "nmc_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Namecoin(NMC/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5da56b968529d.png",
                "new_price": 0.0026,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.0026,
                "max_price": 0.0026,
                "change": 0,
                "volume": 4
            },
            {
                "id": "60",
                "ticker": "dash_pars",
                "fee_buy": "0.05",
                "fee_sell": "0.05",
                "name": "Dash(DASH/PARS)",
                "icon": "http://parsxc.com/Upload/coin/5d8c9f76d8a86.png",
                "new_price": 63000,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 63000,
                "max_price": 63000,
                "change": 0,
                "volume": 0.015
            },
            {
                "id": "62",
                "ticker": "doge_pars",
                "fee_buy": "0.05",
                "fee_sell": "0.05",
                "name": "Dogecoin(DOGE/PARS)",
                "icon": "http://parsxc.com/Upload/coin/5d8ca5867afc2.png",
                "new_price": 0.5,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.5,
                "max_price": 0.5,
                "change": 0,
                "volume": 10
            },
            {
                "id": "91",
                "ticker": "xvg_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Verge(XVG/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5d8d26b41eebc.png",
                "new_price": 0.000019,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.000019,
                "max_price": 0.000019,
                "change": 0,
                "volume": 3
            },
            {
                "id": "71",
                "ticker": "usdt_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Tether(USDT/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5d8d1ca35cef2.png",
                "new_price": 0.000122,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.000122,
                "max_price": 0.000122,
                "change": 0,
                "volume": 10
            },
            {
                "id": "72",
                "ticker": "usdt_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Tether(USDT/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5d8d1ca35cef2.png",
                "new_price": 162,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 162,
                "max_price": 162,
                "change": 0,
                "volume": 0
            },
            {
                "id": "73",
                "ticker": "pars_usdt",
                "fee_buy": "0.05",
                "fee_sell": "0.05",
                "name": "ParsiCoin(PARS/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5da42d4dd5bff.png",
                "new_price": 0.001,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.001,
                "max_price": 0.001,
                "change": 0,
                "volume": 0
            },
            {
                "id": "74",
                "ticker": "ltc_usdt",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Litecoin(LTC/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5d8867471450b.png",
                "new_price": 50,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 50,
                "max_price": 50,
                "change": 0,
                "volume": 0.03
            },
            {
                "id": "75",
                "ticker": "waves_usdt",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Waves(WAVES/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5d8c9d9cc5f5e.png",
                "new_price": 0.715,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.715,
                "max_price": 0.715,
                "change": 0,
                "volume": 2
            },
            {
                "id": "76",
                "ticker": "bch_usdt",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Bitcoin Cash(BCH/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5d8c9e2ca570d.png",
                "new_price": 217,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 217,
                "max_price": 217,
                "change": 0,
                "volume": 0.015
            },
            {
                "id": "80",
                "ticker": "dash_usdt",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Dash(DASH/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5d8c9f76d8a86.png",
                "new_price": 63.5,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 63.5,
                "max_price": 63.5,
                "change": 0,
                "volume": 0.025
            },
            {
                "id": "82",
                "ticker": "doge_usdt",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Dogecoin(DOGE/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5d8ca5867afc2.png",
                "new_price": 0.00254,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.00254,
                "max_price": 0.00254,
                "change": 0,
                "volume": 25
            },
            {
                "id": "85",
                "ticker": "rvn_usdt",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Ravencoin(RVN/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5d8ca7f2e7fd5.png",
                "new_price": 0.0283,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.0283,
                "max_price": 0.0283,
                "change": 0,
                "volume": 9
            },
            {
                "id": "87",
                "ticker": "pivx_usdt",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Pivx(PIVX/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5d8ca8b7f0694.png",
                "new_price": 0.2128,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.2128,
                "max_price": 0.2128,
                "change": 0,
                "volume": 9
            },
            {
                "id": "94",
                "ticker": "xvg_usdt",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Verge(XVG/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5d8d26b41eebc.png",
                "new_price": 0.0032,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.0032,
                "max_price": 0.0032,
                "change": 0,
                "volume": 3
            },
            {
                "id": "89",
                "ticker": "mona_usdt",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Monacoin(MONA/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5d8ca9378c2df.png",
                "new_price": 1,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 1,
                "max_price": 1,
                "change": 0,
                "volume": 2
            },
            {
                "id": "98",
                "ticker": "ppc_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Peercoin(PPC/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5da57f41d1c32.png",
                "new_price": 0.00003,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.00003,
                "max_price": 0.00003,
                "change": -6.42,
                "volume": 4
            },
            {
                "id": "99",
                "ticker": "ppc_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Peercoin(PPC/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5da57f41d1c32.png",
                "new_price": 0.0014,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.0014,
                "max_price": 0.0014,
                "change": 0,
                "volume": 2
            },
            {
                "id": "100",
                "ticker": "ppc_usdt",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Peercoin(PPC/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5da57f41d1c32.png",
                "new_price": 0.229,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.229,
                "max_price": 0.229,
                "change": 0,
                "volume": 4
            },
            {
                "id": "101",
                "ticker": "pac_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Paccoin(PAC/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5da583e15a2b1.png",
                "new_price": 0.00000004,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.00000004,
                "max_price": 0.00000004,
                "change": 0,
                "volume": 3
            },
            {
                "id": "102",
                "ticker": "pac_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Paccoin(PAC/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5da583e15a2b1.png",
                "new_price": 0.0000018,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.0000018,
                "max_price": 0.0000018,
                "change": 0,
                "volume": 3
            },
            {
                "id": "103",
                "ticker": "pac_usdt",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Paccoin(PAC/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5da583e15a2b1.png",
                "new_price": 0.00032,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.00032,
                "max_price": 0.00032,
                "change": 0,
                "volume": 4
            },
            {
                "id": "104",
                "ticker": "waves_pars",
                "fee_buy": "0.05",
                "fee_sell": "0.05",
                "name": "Waves(WAVES/PARS)",
                "icon": "http://parsxc.com/Upload/coin/5d8c9d9cc5f5e.png",
                "new_price": 100,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 100,
                "max_price": 100,
                "change": 0,
                "volume": 2
            },
            {
                "id": "105",
                "ticker": "mona_pars",
                "fee_buy": "0.05",
                "fee_sell": "0.05",
                "name": "Monacoin(MONA/PARS)",
                "icon": "http://parsxc.com/Upload/coin/5d8ca9378c2df.png",
                "new_price": 150,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 150,
                "max_price": 150,
                "change": 0,
                "volume": 2
            },
            {
                "id": "106",
                "ticker": "scavo_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Scavo Token(SCAVO/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5db05340919c6.png",
                "new_price": 0.00000001,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.00000001,
                "max_price": 0.00000001,
                "change": 0,
                "volume": 0
            },
            {
                "id": "107",
                "ticker": "scavo_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Scavo Token(SCAVO/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5db05340919c6.png",
                "new_price": 0,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0,
                "max_price": 0,
                "change": 0,
                "volume": 0
            },
            {
                "id": "108",
                "ticker": "scavo_usdt",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Scavo Token(SCAVO/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5db05340919c6.png",
                "new_price": 0.0001,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.0001,
                "max_price": 0.0001,
                "change": 0,
                "volume": 0
            },
            {
                "id": "109",
                "ticker": "onion_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Deeponion(ONION/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5db184c8dd2fd.png",
                "new_price": 0.000018,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.000018,
                "max_price": 0.000018,
                "change": 0,
                "volume": 2
            },
            {
                "id": "110",
                "ticker": "onion_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Deeponion(ONION/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5db184c8dd2fd.png",
                "new_price": 0.00085,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.00085,
                "max_price": 0.00085,
                "change": 0,
                "volume": 3
            },
            {
                "id": "111",
                "ticker": "onion_usdt",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Deeponion(ONION/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5db184c8dd2fd.png",
                "new_price": 0.1386,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.1386,
                "max_price": 0.1386,
                "change": 0,
                "volume": 5
            },
            {
                "id": "112",
                "ticker": "dgb_btc",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Digibyte(DGB/BTC)",
                "icon": "http://parsxc.com/Upload/coin/5db1d04d2c541.png",
                "new_price": 0.00000091,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.00000091,
                "max_price": 0.00000091,
                "change": 0,
                "volume": 2.5
            },
            {
                "id": "113",
                "ticker": "dgb_eth",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Digibyte(DGB/ETH)",
                "icon": "http://parsxc.com/Upload/coin/5db1d04d2c541.png",
                "new_price": 0.000042,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.000042,
                "max_price": 0.000042,
                "change": 0,
                "volume": 3.5
            },
            {
                "id": "114",
                "ticker": "dgb_usdt",
                "fee_buy": "0.1",
                "fee_sell": "0.1",
                "name": "Digibyte(DGB/USDT)",
                "icon": "http://parsxc.com/Upload/coin/5db1d04d2c541.png",
                "new_price": 0.0068,
                "buy_price": 0,
                "sell_price": 0,
                "min_price": 0.0068,
                "max_price": 0.0068,
                "change": 0,
                "volume": 4
            }
        ]
    }
}
```