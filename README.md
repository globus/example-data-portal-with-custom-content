# Example : Serverless Data Portal with Custom Content

This repository is an example implementation of the [@globus/template-data-portal](https://github.com/globus/template-data-portal).


You can create your own portal with similar functionality by following the [**Creating Your Own Research Data Portal**](https://github.com/globus/template-data-portal?tab=readme-ov-file#creating-your-own-research-data-portal) section in the template repository and then referencing the sections below.


<img width="1409" src="https://github.com/user-attachments/assets/48b088c8-f095-474e-a2fa-e89616d9e5e7">




## Creating a Custom Landing Page

- Create a new file in your repository at `/content/index.md` and add your desired contents.
  - The underlying portal code supports [CommonMark](https://commonmark.org/).
- Commit your changes.
- The template-included GitHub Action will automatically trigger rebuilding your site with the new landing page.

View Example: https://globus.github.io/example-data-portal-with-custom-content/ ([Markdown Source](/content/index.md))


## Hosting Assets

- Create a new directory `/content/assets` and add your desired assets.
- Assets will be hosted at the root of your deployed application.
  - We recommend creating additional directories inside `assets` to avoid conflicts with other pages and general organization, e.g. `/content/assets/images/...`
- When using Markdown, you can reference your assets using a full URL or relative path.

|Asset Path| Relative Reference | Full URL |
|----------|--------------------|----------|
| `/content/assets/example.png` | `![](/example.png)` | `![](https://{username}.github.io/{repository_name}/example.png)` |
| `/content/assets/images/chart.jpg` | `![](/images/chart.jpg)` | `![](https://{username}.github.io/{repository_name}/images/chart.jpg)` |

View Example: https://globus.github.io/example-data-portal-with-custom-content/ ([Markdown Source](/content/index.md), [Assets Source](/content/assets))


## Additional Pages + Routes

The simplest way to add additional pages or routes to your portal is to create additional Markdown (`.md`) files in your content directory. When a new file is added, the page will become accessible at `{HOST}/{CONTENT_RELATIVE_PATH_WITHOUT_EXTENSION}`.

|Content Path| Page URL |
|----------|--------------------|
| `/content/welcome.md` | `{HOST}/welcome`|
| `/content/documentation/how-to.md` | `{HOST}/documentation/how-to`|

View Example: https://globus.github.io/example-data-portal-with-custom-content/documentation/example ([Markdown Source](/content/documentation/example.md))






