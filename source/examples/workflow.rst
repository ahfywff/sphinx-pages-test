Example Workflow
================

::

    on: [push]

    jobs:
      build:
        name: Sphinx Pages Test
        runs-on: ubuntu-latest
        steps:
          - uses: seanzhengw/sphinx-pages@master
            id: sphinx-pages
            with:
              github_token: ${{ secrets.GITHUB_TOKEN }}
              create_readme: true
