# Docky

Docky is a dockerizer application built specifically for e-commerce development environment.  
He helps developer to build up a proper environment that let you just focus and work on only your thing without worrying about setting up server / application.

Basically, Docky works well with **WooCommerce**.

## Usage

_**Clone**_ or [_**download**_](https://github.com/guzzilar/docky/archive/master.zip) the repository to your local machine.  
Then, to run Docky, execute the following command right away in your terminal program:

```bash
bin/docky up [platform]:[version(optional)] [app_name(optional)]
```

> Note: Default of the `version` parameter is `latest`.

For example:
```bash
bin/docky up woocommerce:latest my-woocommerce
```

Docky will create a new folder `app/my-woocommerce`. Then, deploy all build-related files into that folder.

Once finished, mow you will be able to edit or make any changes inside `app/my-woocommerce/html`. It will sync to your container as well.

## Supported platforms

Here is the list of platforms that you can build with Docky:

- [WooCommerce](https://github.com/guzzilar/docky#woocommerce)

### WooCommerce

#### Versions supported

- latest (`bin/docky up woocommerce`)

**Database**  
DB Host: _`db`_  
DB Name: _`www`_  
DB User: _`root`_  
DB Password: _`root`_

**Access**  
`http://127.0.0.1`
