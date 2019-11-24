# 如何获取USDT对人民币汇率？

### 1.用火币的接口获取
GET https://otc-api-sz.eiijo.cn/v1/data/trade-market?coinId=2&currency=1&tradeType=sell&currPage=1&payMethod=0&country=37&blockType=general&online=1&range=0

result.data[0].price就是了

### 2.用okex的接口获取
GET https://www.okex.com/v3/c2c/tradingOrders/book?t=1574598226250&side=sell&baseCurrency=usdt&quoteCurrency=cny&userType=certified&paymentMethod=all

result.data.sell[0].price就是了