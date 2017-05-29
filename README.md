# Docky

Docky is a dockerizer application built specifically for e-commerce development environment.  
He would help developer to build up a proper environment that let you just focus and work on only your thing without caring about server-match-requirement.

Basically, Docky works well with **WooCommerce**, **Magento**, **Magento 2**, **OpenCart**.

## Usage

_**Clone**_ or [_**download**_](https://github.com/guzzilar/docky/archive/master.zip) the repository to your local machine.  
Then, in order to run Docky, execute the following command right away in your terminal program:

```bash
bin/docky up [platform]:[version(optional)]
```

> Note: Default of the `version` parameter is `latest`.

## Supported platforms

Here is the list of platforms that you can build with Docky:
- [EC-Cube](https://github.com/guzzilar/docky#ec-cube)
- [Magento](https://github.com/guzzilar/docky#magento)
- [WooCommerce](https://github.com/guzzilar/docky#woocommerce)

### WooCommerce

#### Versions supported

- latest _`auto install`_

    _example_

    ```bash
    bin/docky up woocommerce
    ```

**Database Informations**

DB Host: `db`  
DB Name: `www`  
DB User: `root`  
DB Password: `root`

Url access: `http://127.0.0.1`

---

### EC-Cube

#### Versions supported

- 2.13.3

    _example_

    ```bash
    bin/docky up eccube:2.13.3
    ```

**Database Informations**

DB Host: db  
DB Name: www  
DB User: postgres  
DB Password: root

Url access: `http://127.0.0.1`

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

**Database Informations**

DB Host: `db`  
DB Name: `www`  
DB User: `root`  
DB Password: `root`

Url access: `http://127.0.0.1`
