This is a site I've created to learn a little bit more about Craft CMS. It's purpose is to be a simple blog style website that can be easily updated by non-dev users. The site consistes of main updates, drink of the month, and local resources.

1. [Install DDEV](https://ddev.readthedocs.io/en/latest/users/install/ddev-installation/)
2. Choose a folder for your project and move into it:
    ```bash
    cd /path/to/web/projects
    mkdir mos
    cd mos
    ```
3. Configure a new DDEV [project](https://ddev.readthedocs.io/en/latest/users/quickstart/#craft-cms), and install Craft:
    ```bash
    ddev config --project-type=craftcms

    # Use this package as a starting point:
    ddev composer create -y --no-scripts --no-install craftcms/craft

    # Boot up your development environment:
    ddev start

    # Install packages:
    ddev composer update

    # Run the Craft CMS installer (use all defaults):
    ddev craft install

    # -> https://my-project.ddev.site/
    ```
4. Visit the URL printed to your terminal, or run `ddev launch`.


## Resources

Craft’s [control panel](https://craftcms.com/docs/4.x/control-panel.html) is located at `/admin`. The rest is up to you! Pick up where we left off in [the tutorial](https://craftcms.com/docs/getting-started-tutorial/configure/control-panel.html), or dive right in on modeling your own content:
- :card_file_box: [Elements](https://craftcms.com/docs/4.x/elements.html): Learn about Craft’s core content types, and how to customize them.
- :triangular_ruler: [Fields](https://craftcms.com/docs/4.x/fields.html): Create precisely the data structure and authoring experience you need.
- :pencil2: [Templating](https://craftcms.com/docs/4.x/dev/twig-primer.html): Start using your data in a totally custom front-end.
