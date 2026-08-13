Remote config for the Maxim Dispatch iOS shell (klakhnath/dispatch-ios).

The app reads config.json on every launch. Deliberately PUBLIC and deliberately not
hosted on the dispatch server — this file must stay reachable when that server is
exactly the thing that's down. It contains no secrets: the base URL is public.

- base_url: where the shell points (change = every installed app follows, no rebuild)
- min_shell_ver: bump above the shipped bridge version to force an upgrade wall
- message: shown with the upgrade wall
