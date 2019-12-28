goods_price = {'stock': 10, 'T-shit': 70, 'jaket': 200, 'pants': 300, 'underdress': 50, 'cup': 20, 'table': 200}
x=goods_price['stock']
def match_price():
    goods_list=list(goods_price.keys())
    price_list=list(goods_price.values())
    for sale_goods in goods_list:
        print(sale_goods)
        i=goods_list[sale_goods]

        price=price_list[i]
        return price
if __name__=='__main__':
    try:
        match_price()
    except TabError as e:
        print('出错了：',e)
