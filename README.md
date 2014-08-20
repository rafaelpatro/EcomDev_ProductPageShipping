EcomDev_ProductPageShipping
===========================

Estimate Shipping on the Product Page

- Install module
- Activate in configuration

To use on product page follow instructions:

- Add on your /template/catalog/product/view.phtml:
```
    <?php echo $this->getChildHtml('shipping.estimate.form'); ?>
```  
- Add on your local.xml
```
    <catalog_product_view>
      <update handle="ecomdev_productpageshipping_skeleton" />
      <reference name="product.info">
        <action method="insert"><block>shipping.estimate.form</block></action>
      </reference>
    </catalog_product_view>
```    
