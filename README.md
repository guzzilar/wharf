# Docky

Docky is a dockerizer application built specifically for e-commerce development.
He helps developer to run up e-commerce dev environments related.
i.e. Magento, WooCommerce, EC-Cube

## Usage

Just `clone` or `download` the repository to your machine.

Then, to run Docky, type the following command to your terminal program:

```bash
bin/docky up [platform]:[version(optional)]
```

> note, default of `version` is `latest`.

## Supported platforms

Here is the list of platforms that you can build with Docky:

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
