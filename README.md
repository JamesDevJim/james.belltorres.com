# James Bell-Torres Professional Site

Single-page Jekyll site for `james.belltorres.com`, built for GitHub Pages with minimal moving parts.

## Local Build

Preferred verification command:

```sh
bundle exec jekyll build
```

This repo intentionally has no custom plugins, collections, frontend framework, or build tooling beyond GitHub Pages-compatible Jekyll.

Build verification note: `bundle exec jekyll build` could not be completed in the migration environment because the fresh repo has no `Gemfile` or `.bundle/` directory, and `jekyll` is not installed globally.

## GitHub Pages Setup

The public GitHub repo was created at:

https://github.com/JamesDevJim/james.belltorres.com

GitHub Pages was configured during migration:

- Source: Deploy from a branch
- Branch/path: `main` / `/root`
- Custom domain: `james.belltorres.com`

If settings ever need to be restored manually:

1. Open Settings -> Pages.
2. Set Source to "Deploy from a branch".
3. Select `main` and `/root`.
4. Save.

## DNS Setup

Create or verify this DNS record:

- Type: CNAME
- Name/host: `james`
- Value/target: `jamesdevjim.github.io`

The repo includes a root `CNAME` file containing `james.belltorres.com`.

## Migration Report

Source visual reference:

- `github.com/JamesDevJim/belltorres.com`
- Reviewed `_layouts/`, `_includes/`, `_config.yml`, and `assets/css/`.
- Reused the general typography, spacing, sticky header, ocean-blue/charcoal palette, and 8px radius convention.
- Did not copy the family-site navigation, feed plugins, sitemap plugins, Google Fonts include, footer social clutter, or unrelated layouts.

Source Staatic files used:

- `/Users/jamesbell/Documents/BuildingEnergyTools/Staatic export/index.html`
- `/Users/jamesbell/Documents/BuildingEnergyTools/Staatic export/about/index.html`
- `/Users/jamesbell/Documents/BuildingEnergyTools/Staatic export/quantification/index.html`

Content extracted:

- Home: building basics prose, 90% time in buildings, 40% U.S. energy consumed by buildings, 39.4 qBTU annual U.S. building energy consumption, the sustainability strategy process, and energy conservation measure labels for schedules, resets, optimization, and repairs.
- About: professional bio positioning, energy and water waste focus, utility incentive program work, demand response/load management, campus energy and water management, lab and GMP facility experience, controls optimization, BAS overrides, FDD, and asset categories.
- Quantification: original equation references for energy, cost, savings, efficiency, heat, electrical power, motors, boilers, chiller COP, water leaks, AHU calculations, and whole-HVAC calculations.
- Tools: a simplified AHU runtime calculator implementing the requested energy, cost, and CO2 formulas in vanilla JavaScript.
- Images: James' professional portrait, three professional fieldwork photos, four stock images, building-energy and strategic-management diagrams, four PNNL energy conservation measure graphics, AHU/HVAC diagrams, and the equation images referenced by the selected source pages.

Content intentionally omitted:

- WordPress, Staatic, Elementor, OceanWP, plugin, shortcode, and `wp-content` markup/classes/scripts.
- Unused theme images, plugin graphics, duplicate WordPress thumbnails, personal/travel/hobby images, and images referenced only by excluded pages.
- Feeds, RSS, sitemaps, XML, `wp-json`, blog posts, archive pages, author/category pages, comments, login/admin references, visualization, quiz/challenge, and kite content.
- References to the retired source domain.
- Personal/family/travel/hobby material and professional testimonials naming other people.

Known TODOs:

- Add James Bell-Torres' exact LinkedIn URL in `index.html`; it was not discoverable in the selected Staatic files or reference repo.
- The selected Staatic home page did not expose exact numeric end-use percentages for HVAC, lighting, or plug loads, so the page uses only the available end-use/opportunity labels.
