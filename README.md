# Docky

Docky is a dockerizer application built specifically for e-commerce development environment.  
He helps developer to build up a proper environment that let you just focus and work on only your thing without worrying about setting up server / application.

Basically, Docky works well with **WooCommerce**, **Magento**, **Magento 2**, **OpenCart**.

## Usage

_**Clone**_ or [_**download**_](https://github.com/guzzilar/docky/archive/master.zip) the repository to your local machine.  
Then, to run Docky, execute the following command right away in your terminal program:

```bash
bin/docky up [platform]:[version(optional)]
```

> Note: Default of the `version` parameter is `latest`.

i.e.
```bash
bin/docky up woocommerce:latest
```

## Supported platforms

Here is the list of platforms that you can build with Docky:
- [EC-Cube](https://github.com/guzzilar/docky#ec-cube)
- [Magento](https://github.com/guzzilar/docky#magento)
- [WooCommerce](https://github.com/guzzilar/docky#woocommerce)

### EC-Cube

#### Versions supported

- 2.13.3 (`bin/docky up eccube:2.13.3`)

**Database**  
DB Host: _`db`_  
DB Name: _`www`_  
DB User: _`postgres`_  
DB Password: _`root`_

**Access**  
`http://127.0.0.1`

---

### Magento

#### Versions supported

- 2.1.6
- 2.1.5
- 1.9.3.2
- 1.9.3.1
- 1.9.2.2

_example_

```bash
bin/docky up magento:1.9.3.1 --source=directory/of/file/magento1.9.3.1.zip
```

> Because Docky cannot access to Magento v1.x resources without log in to Magento website.  
> 
> So, you have to manually log in and download a zip file directly from https://magento.com/tech-resources/download. And then, specify a path of a zip file you download (unfortunately, Docky cannot do automatically download task for you).

**Database**  
DB Host: _`db`_  
DB Name: _`www`_  
DB User: _`root`_  
DB Password: _`root`_

**Access**  
`http://127.0.0.1`

---

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
