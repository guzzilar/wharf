# Docky

Docky is a dockerizer application to help developer run up various dev servers.

## Usage

Just clone/download the repository to your machine.

Then, to run Docky, type the following commands to your terminal program:

```bash
bin/docky build [platform]:[version(optional)]
```

> note, default of `version` is `latest`.

## Supported platforms

Here is the list of platforms that you can build with Docky:

### WooCommerce

#### Versions supported

- latest

    ```bash
    bin/docky build woocommerce
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

    ```bash
    bin/docky build eccube:2.13.3
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

- 1.9.3.1

    ```bash
    bin/docky build magento:1.9.3.1 --source=directory/of/file/magento1.9.3.1.zip
    ```

    > Because Docky cannot access to Magento v1.x resources without log in to Magento website.  
    >
    > So, you have to manually log in and download a zip file directly from https://magento.com/tech-resources/download. And then, specify a path of a zip file you download (unfortunately, Docky cannot do automatically download task for you).

**Database Informations**

DB Host: db  
DB Name: www  
DB User: root  
DB Password: root

Url access: `http://127.0.0.1`
