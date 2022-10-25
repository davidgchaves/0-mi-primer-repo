# 1 Instalación de programas en Ubuntu

![Cute Cat](./img/cute-cat.jpeg)

## 1.1 `apt`

### 1.1.1 Instalando `git` con `apt`

Para **instalar un programa** en Ubuntu (por exemplo `git`) podemos utilizar o comando `apt`

```sh
sudo apt install git
```

### 1.1.2 Pero qué versión?

O problema de instalar `git` tal e como se detalla no 1.1.1, é que a versión instalada e bastante antigua. Se queremos instalar un versión reciente, debemos engadir un repositorio `ppa` externo a Ubuntu (**co risco de seguridade asociado**).

### 1.1.3 `add-apt-repository`

Co seguinte comando podemos engadir o **repositorio `ppa`** do [_"Ubuntu Git Maintainers" team_](https://launchpad.net/~git-core/+archive/ubuntu/ppa).

> The most current stable version of Git for Ubuntu.
>
> For release candidates, go to https://launchpad.net/~git-core/+archive/candidate.

```sh
sudo add-apt-repository ppa:git-core/ppa
```

**NOTA**: recordamos, novamente, que trátase dun repositorio `ppa` alleo a Ubuntu, e por tanto un potencial problema de seguridade.

A continuación simplemente temos que executar os seguintes comandos

```sh
sudo apt update
sudo apt install git
```

Con esto instalaremos a versión de `git` máis reciente para o nos sistema.

### 1.1.4 Versións `git`

| Repo                 | `git --version`      |
|----------------------|----------------------|
| Focal (Ubuntu 20.04) | `git version 2.25.1` |
| PPA Git Maintainers  | `git version 2.37.3` |

Taboa cortesía de [**Tables Generator**](https://www.tablesgenerator.com/markdown_tables)

