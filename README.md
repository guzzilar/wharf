# Docky

Docky is a dockerizer application built specifically for runnig up e-commerce applications (for development purpose).  
He helps developer to build up a proper environment that let you just focus and work on only your thing without worrying about setting up server / application.

### Here is the list of e-commerce platforms that Docky can work with:

- [WooCommerce](https://github.com/guzzilar/docky#woocommerce)

**Future Plan**  
Magento, EC-Cube, PrestaShop, OpenCart are coming!

## Usage

_**Clone**_ or [_**download**_](https://github.com/guzzilar/docky/archive/master.zip) the repository into your local machine.  
Then, to run Docky, execute the following command right away in your terminal program:

```bash
bin/docky up [platform][:version(optional)] [app_name(optional)]
```

> Note: Default of the `version` parameter is `latest`.

#### Example:
```bash
bin/docky up woocommerce:latest my-woocommerce
```

Docky will create a new folder `app/my-woocommerce`. Then, deploy all build-related files into a folder you've assigned.

Once finished, you will be able to edit or make any changes inside `app/my-woocommerce/html`. It will sync automatically to your Docker container as well.

<img width="1403" alt="01" src="https://user-images.githubusercontent.com/2154669/28490968-eaed3b88-6f10-11e7-9fca-dbae7a5ca2f4.png">

## Container Details

### WooCommerce

#### Versions Supported

- latest (`bin/docky up woocommerce`)

**Database**  
DB Host: _`db`_  
DB Name: _`www`_  
DB User: _`root`_  
DB Password: _`root`_

**Access**  
`http://127.0.0.1`
