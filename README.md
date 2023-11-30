class Ecommerce:
    def __init__(self, name, products=[]):
        self.name = name
        self.products = products

    def add_product(self, product):
        self.products.append(product)
        print(f"{product} added to {self.name}")

    def list_products(self):
        print(f"Products available in {self.name}:")
        for product in self.products:
            print(f"- {product}")

# Example usage:
if __name__ == "__main__":
    my_ecommerce = Ecommerce("MyStore")
    
    my_ecommerce.add_product("Laptop")
    my_ecommerce.add_product("Smartphone")
    
    my_ecommerce.list_products()
