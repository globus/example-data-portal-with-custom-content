# Example : Serverless Data Portal with Custom Content

This repository is an example implementation of the [@globus/template-data-portal](https://github.com/globus/template-data-portal).

You can create your own portal with similar functionality by following the [**Creating Your Own Research Data Portal**](https://github.com/globus/template-data-portal?tab=readme-ov-file#creating-your-own-research-data-portal) section in the template repository and then making the following modifications:


## Creating a Custom Landing Page

- Create a new file in your repository at `/content/index.md` and add your desired contents.
  - The underlying portal code supports [CommonMark](https://commonmark.org/).
- Commit your changes.
- The template-included GitHub Action will automatically trigger rebuilding your site with the new landing page.

View Example: https://globus.github.io/example-data-portal-with-custom-content/ ([source](/content/index.md))


