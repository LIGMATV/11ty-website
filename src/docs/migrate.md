---
eleventyNavigation:
  parent: Getting Started
  key: Migrating to Eleventy
  order: 3
---

# {{ eleventyNavigation.key }}

## Tools

- [`@11ty/import`](https://github.com/11ty/eleventy-import) is a command line tool to import from various data sources as static content files in your project.
	- You can [use `@11ty/import` to import your WordPress blog](/docs/migrate/wordpress/#use-@11ty/import)

## Guides

<ul class="list-bare">
{%- for post in collections.migrations %}
	<li><a href="{{ post.url }}">{% if post.data.iconUrl %}{% indieavatar post.data.iconUrl %}{% endif %}{{ post.data.title }}</a></li>
{%- endfor %}
</ul>