<p align="center">
  <a>
    <img src="public/images/logo-icon.png" alt="Logo" width="80" >
  </a>
</p>

<h1 align="center">Galaxy Swiss Bourdin <a href="https://symfony.com/">Symfony</a></h1>

<p align="center">
  <p align="center">
      GSB is a web App using Symfony framework and depending on twig template. This App is an expense management App for medical field professionals.
  </p> 
  <p align="center">
    <a href="https://github.com/hugo-HDSF/GSB_symfony/blob/main/assets/videos/exemple.gif"><strong>View Exemple »</strong></a>
    .
    <a href="https://github.com/hugo-HDSF/GSB_symfony/issues">Report Bug</a>
  </p>
</p>

<div align="center">

![Composer](https://img.shields.io/badge/-Composer_1.11-885630?logo=composer&logoColor=white)
![Symfony](https://img.shields.io/badge/-Symfony_4.4-000000?logo=symfony&logoColor=white)
![PHP](https://img.shields.io/badge/-PHP_8.1-777BB4?logo=php&logoColor=white)
![Doctrine](https://img.shields.io/badge/-Doctrine_2.7-F05032?logo=doctrine&logoColor=white)
![MySQL](https://img.shields.io/badge/-MySQL_5.7-4479A1?logo=mysql&logoColor=white)
![PhpStorm](https://img.shields.io/badge/-PhpStorm-000000?logo=phpstorm&logoColor=white)
</div>

<div align="center">

![Twig](https://img.shields.io/badge/-Twig_3.0-bfcf28?logo=twig&logoColor=black)
![Bulma](https://img.shields.io/badge/-Bulma_0.9.3-00D1B2?logo=bulma&logoColor=white)
![JQuery](https://img.shields.io/badge/-JQuery_3.5.1-0769AD?logo=jquery&logoColor=white)
![Font Awesome](https://img.shields.io/badge/-FontAwesome-528DD7?logo=FontAwesome&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/-HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/-CSS3-1572B6?logo=css3&logoColor=white)
</div>

-----

## Table Of Contents

* [About the Project](#about-the-project)
* [Implementation](#implementation)
* [Built With](#built-with)
* [Getting Started](#getting-started)
    * [Prerequisites](#prerequisites)
    * [Installation](#installation)
* [Usage](#usage)
    * [Target and Source variables](#target-and-source-variables)
    * [Control variables](#control-variables)
* [Roadmap](#roadmap)
* [License](#license)
* [Authors](#authors)
* [Acknowledgements](#acknowledgements)

## About The Project

![Screen Shot](assets/videos/exemple.gif)

This App is an Expense management application for medical professionals. It allows employees to manage their expenses and associated costs during their business trip.

## Implementation

> `🚀 Continuous integration`

## Built With

* [Symfony](https://symfony.com/)
* [Composer](https://getcomposer.org/)
* [Bulma](https://bulma.io/)
* [Twig](https://twig.symfony.com/)
* [JQuery](https://jquery.com/)
* [Font Awesome](https://fontawesome.com/)
* [Doctrine](https://www.doctrine-project.org/)
* [MySQL](https://www.mysql.com/fr/)

## Getting Started

To get a local copy up and running, follow these simple steps:

### Prerequisites

#### 1. Clone repository

```Shell
git clone https://github.com/hugo-HDSF/GSB_symfony.git
```

#### 2. Install dependencies

- Navigate into the cloned project directory and install the project dependencies:

```Shell
cd gsb_symfony
composer install
```

- Copy the .env.dist file to .env:

```Shell
cp .env.dist .env
```

#### 4. Set Up the Database

- functional database listening on 3306 port is needed. we recommend you to install MariaDB 10.5.12 or MySQL 5.7.33.

> **Note**
> MariaDB provieds a full installation [guide](https://mariadb.com/kb/en/getting-installing-and-upgrading-mariadb/) throught their website.

------

#### ___EXEMPLE___

- Connect to your database (acording to your credentials):

```Shell
mariadb -u root -p
```

- Create the database:

```sql
source
db/gsb_structure.sql
```

- Create a new user and grant him all privileges:

```sql
CREATE USER 'gsbadmin'@'localhost' IDENTIFIED BY 'gsb2021';
GRANT ALL PRIVILEGES ON *.* TO 'gsbadmin'@'localhost';
FLUSH PRIVILEGES;
```

- Populate the database and exit the database:

```sql
source
db/gsb_peupler.sql
exit
```

------

#### 5. Run the server

- Generate the SSL certificate:

```Shell
symfony server:ca:install
```

- Start the symfony server:

```Shell
symfony server:start
```

#### 6. Open your browser and navigate to https://localhost:8000

> **Warning**
> credentials are necessary to connect, you can find credentials profils [here](db/gsb_peupler.sql).

## Roadmap

Check list of known [open issues](https://github.com/hugo-HDSF/GSB_symfony/issues).

## License

Distributed under the MIT License.

## Authors

* **DA SILVA Hugo** - *Student - Fullstack Developer* - [Github](https://github.com/hugo-HDSF/)

## Acknowledgements

* [Lycée Louis Armand](https://www.larmand.fr/)
* [Img Shields](https://shields.io/)
* [Simple Icons](https://simpleicons.org/)
* [Readme Generator](https://readme.shaankhan.dev/)

###### _Study Project | (HND) 2021-2022_
