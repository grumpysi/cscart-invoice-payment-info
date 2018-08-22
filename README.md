# CS-Cart Addon - Enable payment_info array in document templates

## Installation
- Download latest release zip file.
- Install zip file via the addon page in the CS-Cart control panel.
## Description
This will enable the additional payment information to be accessible in the document template editor.  So you can use the PO Number on the invoice template for example.

## Development Simlinks
From root of site create plugins folder with a folder called 'invoice_payment_info'
``` 
mkdir plugins/invoice_payment_info/
```

Simlink the main App addon folder
```
cd app/addons
ln -s ../../plugins/invoice_payment_info/app/addons/invoice_payment_info invoice_payment_info
```

Simlink the backend 'css' addon folder
```
cd design/backend/css/addons
ln -s ../../../../plugins/invoice_payment_info/design/backend/css/addons/invoice_payment_info invoice_payment_info
```

Simlink the backend 'media' addon folder
```
cd design/backend/media/images/addons
ln -s ../../../../../plugins/invoice_payment_info/design/backend/media/images/addons/invoice_payment_info invoice_payment_info
```

Simlink the backend 'templates' addon folder
```
cd design/backend/templates/addons
ln -s ../../../../plugins/invoice_payment_info/design/backend/templates/addons/invoice_payment_info invoice_payment_info
```

Simlink the 'var/langs/en' addon folder
```
cd var/langs/en/addons
ln -s ../../../../plugins/invoice_payment_info/var/langs/en/addons/invoice_payment_info.po invoice_payment_info.po
```
