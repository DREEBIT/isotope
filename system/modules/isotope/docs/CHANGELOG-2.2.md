Isotope eCommerce Changelog
===========================

Version 2.2.5-stable (2015-06-16)
---------------------------------

### Fixed
- Options from table were not sorted in cumulative filter


Version 2.2.4-stable (2015-05-12)
---------------------------------

### Improved
- Correctly show/hide tinyMCE 4 when using fallback value for variant attribute (#1335)

### Fixed
- CSS class of messages module was inconsistent (mod_iso_message vs. mod_iso_messages)


Version 2.2.3-stable (2015-03-17)
---------------------------------

### Improved
- Only generate messages module if necessary (fixes #1374)

### Fixed
- Gallery watermark positions were not available in Contao 3.4 (#1365)
- Labels for foreignKey fields were not shown in product attribute view (#1389)
- Manual product sorting (drag&drop) was broken in 2.2.1 (#1388)


Version 2.2.2-stable (2015-02-10)
---------------------------------

### Improved
- Backend product images are resized proportionally instead of cropped

### Fixed
- Product filter did not support attribute options from foreignKey
- Product links did not always point to pages in the current root (#1346)


Version 2.2.1-stable (2015-01-20)
---------------------------------

### Fixed
- Custom template for gallery was not correctly set (#1321)
- Labels were not correctly translated in order PDF and backend notifications (#1325)
- Attributes with options from products can't be filtered in frontend or backend (#1319)


Version 2.2.0-stable (2014-11-24)
---------------------------------

### Improved
- Added post-action hooks to product collection (#1292)
- PayPal IPN should be retried if there's a communication problem with PayPal servers (#1418)

### Fixed
- Checkout step "address" could not be completed when a member was logged in (#1271)
- Duplicating attribute did not copy the attribute options (#1265)
- Rules were not applied to orders (#1290)
- PSP payment was completed without successful postsale request (#1308)
- Incorrect labels in product type when having multiple customer defined fields with options source "product" (#1291)
- Options of multiple products where shown in all attributes (#1291)
- Labels for attribute options were not visible in backend and documents (#1297)


Version 2.2.0-rc1 (2014-10-07)
--------------------------------

### New
- Added the an integrity check to check for attribute option orphans (#1237)
- Added price surcharges for attribute options (#1165)
- Added module to set address before checkout (e.g. for price or shipping calculation)
- Added shipping calculation module (#1187)
- Added condition to payment and shipping restriction on product type
- Added inline edit option for advanced prices
- Added payment method for Billpay (using Saferpay gateway)
- Payment and shipping methods can now handle on order status updates
- Saferpay payment method can now capture/cancel payment on order status change

### Improved
- Performance when finding the correct jumpTo page (#1104)
- Redirect message for payment methods when JavaScript is disabled (#1079)
- Better error logging on invalid PayPal email (#1252)
- Allow to pass attribute options in product collection template

### Fixed
- Warning when product attribute had no options
- Address ID was not correctly update in product collection (#1263)
- Show labels from attribute option table in backend filters (#1253)
- Attribute options from manager were not filterable in the frontend (#1253)


Version 2.2.0-beta1 (2014-09-02)
--------------------------------

### New
- Added the Integrity Check tool to check for database inconsistency
- Integrated payment provider Paybyway from Finland (https://www.paybyway.com)
- Added media player (audio/video) attribute (#1072)
- Added interfaces for attributes with options and variant attributes
- Added placeholder and minlength options to attributes (#1014)
- Payment and shipping methods can be restricted to shop configurations (#1173)
- Galleries can now have custom templates (#1194)
- Dropped support for Contao 3.2 (#1206)
- Added collection_* Simple Token for orders (#1195)
- Support for custom template for every Isotope front end module (#1191)
- Cart does no longer show shipping and payment surcharges (#1055)
- An order collection is created and locked when "buy now" button is pressed

### Improved
- Product options are now available in calculatePrice hook (#1000)
- Show a hint about module configuration when manually sorting products (#1178)
- No need to add an order details front end module to see order details in back end anymore
- Show source collection (cart) ID in the order backend view (#1208)
- Use a template to generate Sparkasse payment URL (#1207)
- Switched to the new Sparkasse payment URL (#1143)
- Isotope shop configuration template folders are now displayed the same way as in Contao core (#1191)
- The backend shop config intro is now responsive (#1221)
- Load page and language environment when sending order notification from backend (#1242)
- Load page and language environment when generating PDF (related to #1242)
