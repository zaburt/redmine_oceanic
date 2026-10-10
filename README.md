# Oceanic

A bright, playful Redmine theme: azure-to-aqua chrome, clean light panels, and
orange, purple and cyan accents, with a speech-bubble logo.

## Installation

1. Clone this theme ([https://github.com/zaburt/redmine_oceanic](https://github.com/zaburt/redmine_oceanic)) into the Redmine `themes/`
   directory at the application root (Redmine 7+) as `oceanic`:

   ```
   git clone https://github.com/zaburt/redmine_oceanic.git themes/oceanic
   ```

   The result should contain:

   ```
   themes/oceanic/stylesheets/application.css
   ```

   > Note: Redmine 6 and earlier used `public/themes/` instead of `themes/`.

2. Restart Redmine. In production, precompile assets:

   ```
   RAILS_ENV=production bin/rails assets:precompile
   ```

3. Go to `Administration -> Settings -> Display` and select "Oceanic"
   in the "Theme" drop-down list.

## Customize

1. Change `images/logo.svg` for the header logo, `images/logo-login.svg` for
   the login page and `favicon/favicon.svg` for the browser tab icon.
2. The palette is defined inline as hex values in
   `stylesheets/application.css`:

   | Role                     | Color     |
   |--------------------------|-----------|
   | Azure (base, links)      | `#0070C0` |
   | Aqua (header end)        | `#0AA6D2` |
   | Orange (actions)         | `#F5710E` / `#D95F00` |
   | Amber                    | `#FFC72C` |
   | Purple (accent)          | `#6B4BE4` |
   | Navy (text)              | `#1B1745` |

   The main menu items are individual pastel color boxes cycling cyan,
   amber, lilac and peach. Surfaces are light tints of azure.
3. In production, re-run `assets:precompile` after editing any theme file.

## License

Licensed under [GNU GPLv2](LICENSE).

Copyright (c) 2026 Onur Küçük (onur [at] delipenguen.net)
