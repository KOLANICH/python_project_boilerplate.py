{{cookiecutter.package_name}}.py [![Unlicensed work](https://raw.githubusercontent.com/unlicense/unlicense.org/master/static/favicon.png)](https://unlicense.org/)
================================
~~[wheel (GitLab)](https://gitlab.com/{{cookiecutter.vcs_hosting_namespace}}/{{cookiecutter.package_name}}.py/-/jobs/artifacts/master/raw/dist/{{cookiecutter.package_name}}-0.CI-py3-none-any.whl?job=build)~~
[wheel (GHA via `nightly.link`)](https://nightly.link/{{cookiecutter.vcs_hosting_namespace}}/{{cookiecutter.package_name}}.py/workflows/CI/master/{{cookiecutter.package_name}}-0.CI-py3-none-any.whl)
~~![GitLab Build Status](https://gitlab.com/{{cookiecutter.vcs_hosting_namespace}}/{{cookiecutter.package_name}}.py/badges/master/pipeline.svg)~~
~~![GitLab Coverage](https://gitlab.com/{{cookiecutter.vcs_hosting_namespace}}/{{cookiecutter.package_name}}.py/badges/master/coverage.svg)~~
[![GitHub Actions](https://github.com/{{cookiecutter.vcs_hosting_namespace}}/{{cookiecutter.package_name}}.py/workflows/CI/badge.svg)](https://github.com/{{cookiecutter.vcs_hosting_namespace}}/{{cookiecutter.package_name}}.py/actions/)
![N∅ hard dependencies](https://shields.io/badge/-N∅_Ъ_deps!-0F0)
[![Libraries.io Status](https://img.shields.io/librariesio/github/{{cookiecutter.vcs_hosting_namespace}}/{{cookiecutter.package_name}}.py.svg)](https://libraries.io/github/{{cookiecutter.vcs_hosting_namespace}}/{{cookiecutter.package_name}}.py)
[![Code style: antiflash](https://img.shields.io/badge/code%20style-antiflash-FFF.svg)](https://github.com/KOLANICH-tools/antiflash.py)

This repo is intended to be used as a [GitHub template repo](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template).

You can apply it without involving `cookiecutter` [(which has grave security issues)](https://github.com/cookiecutter/cookiecutter/issues/429) using the following bash script (fill in it with your data)

```bash
find ./ -maxdepth 1 -type f \( -name "*.md" -o -name "*.yml" -o -name "*.cfg" -o -name "*.toml" \) -exec sed -i 's/{{cookiecutter.author}}/KOLANICH/g; s/{{cookiecutter.vcs_hosting_namespace}}/KOLANICH-libs/g; s/{{cookiecutter.package_name}}/{{cookiecutter.package_name}}/g;' {} \;
sed -i 's/{{cookiecutter.package_name}}/{{cookiecutter.package_name}}/g;' ./tests/tests.py;
```

If you need a `cookiecutter`-based solution, here it is: https://github.com/KOLANICH/python_project_boilerplate_cookiecutter , but it doesn't work currently because of defects in `cookiecutter`.
