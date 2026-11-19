# clashverge



## Clash Verge Rev — A Modern Desktop Client for Clash Meta



Clash Verge Rev is a Tauri 2 based desktop GUI client for [clash verge](https://clashhverge.com/), built on top of the Clash Meta core. It gives Windows, macOS and Linux users a clean, reliable way to manage proxy profiles, rules and subscriptions without touching a terminal. Whether you need to route a single browser through a remote proxy or build complex rule sets for a whole team, Clash Verge Rev keeps every switch, rule and statistic in one well organised place.



[![Clash Verge Rev on Windows](https://clashhverge.com/install-windows.webp)](https://clashhverge.com/)



## Why people choose Clash Verge Rev



Cross platform support means one interface on Windows, macOS and Linux. The Clash Meta core brings full support for TUN mode, Fake-IP, rule providers and TProxy. Profile management lets you import subscription links, merge configs and switch between them in seconds. Traffic insight shows live upload and download charts plus per-connection details. Rules and groups can be edited from the UI, with fallback and url-test policies available without writing YAML by hand.



## Installing on Windows



The Windows build ships as a signed installer. Download the latest setup package from [clash verge github](https://clashhverge.com/) releases, run it, and the tray icon appears next to the clock. TUN mode can be enabled from the settings panel in one click; the client asks for elevation and installs the service automatically. After that every application on the machine, including games and command line tools, goes through the rules you configured.



[![Clash Verge Rev on Windows guide](https://clashhverge.com/install-windows.webp)](https://clashhverge.com/)



## Installing on macOS



macOS users download the universal DMG. Drag the app into Applications, allow it in System Settings, Privacy and Security, then grant network extension permissions the first time TUN mode is switched on. Apple Silicon and Intel binaries are bundled together, so there is no guessing which build to pick. The menu bar item shows the current mode, active profile and traffic counters without opening the main window.



[![Clash Verge Rev on macOS](https://clashhverge.com/install-mac.webp)](https://clashhverge.com/)



## Installing on Linux



On Linux the project provides AppImage, deb and rpm packages. The AppImage is the simplest option: mark it executable, run it, and the GUI talks to the Clash Meta core through a local socket. Service mode installs a systemd unit for transparent proxying. Because every platform uses the same configuration format, a profile exported on Windows works unchanged on a Linux laptop.



## Working with profiles



A profile is simply a YAML configuration that lists proxies, proxy groups and routing rules. In Clash Verge Rev you paste a subscription URL, pick a name and the app downloads, caches and refreshes it on a schedule. You can keep several profiles around and switch between them from the tray menu. A merge profile lets you override just a few keys, for example adding a custom rule provider or changing the DNS settings, while everything else still comes from the remote subscription. This makes it easy to share a base configuration with the rest of a team while each person keeps personal tweaks in a small local overlay.



## Routing and rules



The rule engine decides which outbound a connection uses. Simple setups route everything through one proxy group, but Clash Verge Rev exposes the full rule syntax: domain suffixes, IP ranges, process names, geosite and geoip categories and logical combinations. Rule providers let you pull large lists from a URL and update them automatically. Proxy groups support select, url-test, fallback and load-balance strategies, and each group is editable directly in the GUI so you can reorder or change a policy without editing text files.



## Traffic and diagnostics



The connections page lists every active socket with its host, rule, proxy chain and transferred bytes. You can close a single connection or all of them. The overview page charts upload and download speed over time and shows total traffic for the session. Logs can be filtered by level and searched, which helps when a rule does not match as expected or when a subscription URL is unreachable.



## TUN mode and system proxy



With TUN mode enabled the client creates a virtual network interface and routes traffic from every application through the core, no matter whether the program respects system proxy settings. This is essential for tools, games and containers that ignore environment variables. On the other side, the system proxy mode is lighter and works well on managed machines where installing a service is not allowed. Clash Verge Rev l
