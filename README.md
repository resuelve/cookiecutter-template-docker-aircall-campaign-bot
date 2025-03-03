# cookiecutter-template-docker-aircall-campaign-bot
In this repository, we can find template for lauch aircall-campaign-bot apps using cookiecutter properties

# cookiecutter-template-docker-aircall-campaign-bot

By using this template you can generate a project directory with the follow:

* **README.md**: Custom readme with usage instructions
* **docker-compose**: Custom docker compose service for aircall-campaign-bot

## Install

You need to install `cookiecutter` on your local with another testing tools:

``` shell
$ brew install cookiecutter
```

Additional you can use `yamllint` to validate that the generated manifests are valid.

``` shell
$ brew install yamllint
```

## Usage

Generate a template:

``` shell
$ cookiecutter git@github.com:resuelve/cookiecutter-template-docker-aircall-campaign-bot.git
```

This command will ask you for your project attributes, and after that
creates a directory with your project's name, for example:

``` shell
$ find example-api
example-api
example-api/README.md
example-api/docker-compose.yml

```

### Test resulting yaml

You can use `yamllint` to lint your resulting Github actions workflow, for example:

```shell
$ yamllint example-api/docker-compose.yml
```

Remember to test locally and fix any error reported by the linter before commit.

### Usage for CD workflows

If you wan to build this inside your CI/CD process using Github actions, you can
run cookiecutter without user intervention:

``` shell
$ cd data/vcs
$ cookiecutter git@github.com/resuelve/cookiecutter-template-docker-aircall-campaign-bot.git \
  --no-input \
  --overwrite-if-exists \
  project_name=example-api
```
### Contributions

I you find this useful please send me a kitty image :P, I'm just kidding, just try to use it and give feedback.

### References

Please read the follow references for more details:

* [Cookicutter home](https://github.com/cookiecutter/cookiecutter)
* [Cookicutter documentation](https://cookiecutter.readthedocs.io/en/stable/)
