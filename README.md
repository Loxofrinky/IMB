# IMB
inventory = {
    101: {"Product name": "SALVON HANDWASH",      "Price" :70, "In stock items" : 50},
    102: {"Product name": "PEANUTS",              "Price": 45, "In stock items": 80},
    103: {"Product name": "BESAN POWDER",         "Price": 35, "In stock items": 40}, 
    104: {"Product name": "HALDI POWDER",         "Price": 25, "In stock items": 20}, 
    105: {"Product name": "B0URDON BISCUITS",     "Price": 30, "In stock items": 70}, 
    106: {"Product name": "COLGATE TOOTHPASTE",   "Price": 35, "In stock items": 90}, 
    107: {"Product name": "MARIGOLD BISCUITS",    "Price": 30, "In stock items": 55}, 
    108: {"Product name": "LAYS CLASSICS",        "Price": 20, "In stock items": 67}, 
    109: {"Product name": "AIR SANITISER",        "Price": 50, "In stock items": 98}, 
    110: {"Product name": "MIXED FRUIT JAM",      "Price": 200, "In stock items": 40}, 
    111: {"Product name": "ALAMONDS",             "Price": 135, "In stock items": 234}, 
    112: {"Product name": "PANEER PACKET",        "Price": 130, "In stock items": 189}, 
    113: {"Product name": "SUNFLOWER OIL",        "Price": 160, "In stock items": 210},
    114: {"Product name": "MOONG DAL",            "Price": 40, "In stock items": 231}, 
    115: {"Product name": "VASELINE",             "Price": 15, "In stock items": 321}, 
    116: {"Product name": "EAR BUDS",             "Price": 20, "In stock items": 80}, 
    117: {"Product name": "MAGGI NOODLES",        "Price": 120, "In stock items": 170}, 
    118: {"Product name": "WHITE PEAS",           "Price": 50, "In stock items": 50}, 
    119: {"Product name": "SOFFOLA OATS",         "Price": 75, "In stock items": 80}, 
    120: {"Product name": "LITE POHA",            "Price": 200, "In stock items": 320}, 
    121: {"Product name": "GROUNDNUT OIL",        "Price": 160, "In stock items": 90}, 
    122: {"Product name": "KISSAN KETCHUP" ,       "Price": 25, "In stock items": 50}, 
    123: {"Product name": "MINI SOYA CHUNKS",     "Price": 30, "In stock items": 430}, 
    124: {"Product name": "GIELETTE SHAVESLIDES", "Price": 15, "In stock items": 60}, 
    125: {"Product name": "CANDLES",              "Price": 30, "In stock items": 80}, 
    126: {"Product name": "PAAPPAD",              "Price": 20, "In stock items": 398}, 
    127: {"Product name": "HAKKA NOODLES",        "Price": 90, "In stock items": 234}, 
    128: {"Product name": "DARK FANTASY",         "Price": 100, "In stock items": 411},
    129: {"Product name": "VERMICELLI",           "Price": 100, "In stock items": 59}, 
    130: {"Product name": "DRY FRUITS",           "Price": 40, "In stock items": 89}
    
}    
ui_product = int(input("Enter product ID:"))
ui_quantity = int(input("Enter Quantity:"))

product = inventory.get(ui_product)

if product:
  print('product name: ',product.get('Product name'))
  print('price per unit: ', product.get('Price'))
  print('total amount : ', int(ui_quantity)*(product.get('Price')))
  product['In stock items']-=ui_quantity
else:
  print('product not found')
  
  Enter product ID:129
Enter Quantity:2
product name:  VERMICELLI
price per unit:  100
total amount :  200

