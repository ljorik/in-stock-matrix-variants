# in-stock-matrix-variants
trying to find a solution on the conform plus default theme to only display in-stock matrix variants, if i find a solution everyone with the same problem can use this if they want.

<form action="{{ ('cart/add/' ~ product.vid) | url }}" id="product_configure_form" method="post">
      {% if product.options or product.variants or product.custom %}
      <div class="product-option row">
       <div class="col-md-12">
      {{ product | html_product_configure | raw }}
