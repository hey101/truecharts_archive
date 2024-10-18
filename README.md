# TrueNAS SCALE catalog

This is a fork of the archived TrueCharts App Catalog for TrueNAS SCALE.

Since iX-Systems will deprecate their Kubernets/Helm-based GUI app plattform in Q4 2024, TrueCharts already deprecated their TrueNAS catalog. Thus, you cannot update your already installed applications anymore although there's currently no migration to another Kubernetes plattform available. There will be a migration to their new Kubernetes-based plattform(s).  
But for now, you have to wait.

Therefore I decided to fork their archived chart repository and manually push some updates for applications I personally use. Feel free to use this chart to update your own TrueCharts applications on TrueNAS SCALE.

&nbsp;

### **Be aware that I won't continue pushing updates as soon as there's a stable migration to a new Kubernetes/Helm plattform available!**

### **!!! I am not responsible for any issues that might occur. Always backup your data! !!!**

&nbsp;

- ### How to change your TrueCharts catalog:
    
    1.  Remove your already old/deprecated TrueCharts catalog: *Apps* --> *Discover Apps* --> *Manage Catalogs* --> *TRUECHARTS* --> *Delete* (don't worry, this won't delete any of your already installed applications)
    2.  Add this repository as a new Catalog:
        1.  *Add Catalog* --> *Continue*
            - **Catalog Name:** TrueCharts
            - **Repository:** https://github.com/hey101/truecharts_archive
            - **Preferred Trains:** incubator, premium, stable, system
            - **Branch:** main

Now you should be able to update your applications again.

- ### I made a script that automatically updates all applications based on the manual update method that v3DJG6GL used on his chart. I can't guarantee that something will not break, but it at least works for the apps I use and saves the manual update time. This does not account for using other images instead of the ones truechart uses. I need to add a method for working around this if there are issues. If you have any problems, just create a new issue and I will see what I can do. 


- ### Changelog:
	- 2024.10.18 @ 12:33 PM EST:
		- Stable:
			- acestream: v2.0.2.8 --> v2.1.1.1
			- anki-sync-server: v1.1.14 --> v1.1.4
			- calibre: v7.19.0 --> v7.20.0
			- convos: vstable --> v8.07
			- ghostfolio: v2.115.0 --> v2.116.0
			- home-assistant: v2024.10.2 --> v2024.10.3
			- jackett: v0.22.809 --> v0.22.812
			- scrypted: v0.119.3 --> v0.121.0
			- strapi: v4.16.2 --> v4.25.11
		- Incubator:
			- pingvin-share: v1.2.1 --> v1.2.2
			- semaphore: v2.19.10 --> v2.10.30
			- victoriametrics: v1.104.0 --> v1.105.0
	- 2024.10.18 @ 03:11 AM EST:
		- Stable:
			- gravity: v0.9.1 --> v0.9.3
			- scrypted: v0.119.2 --> v0.119.3
			- sourcegraph: v5.8.1579 --> v5.8.1757
			- unmanic: v0.2.7 --> v0.2.8
	- 2024.10.17 @ 01:11 PM EST:
		- Stable:
			- ddns-go: v6.7.1 --> v6.7.2
			- homer: v24.05.1 --> v24.10.1
			- jackett: v0.22.806 --> v0.22.809
			- onlyoffice-document-server: v8.1.3 --> v8.2.0
			- shlink: v4.2.2 --> v4.2.3
			- smtp-relay: v0.5.6 --> v0.5.7
			- zwavejs2mqtt: v9.23.0 --> v9.24.0
	- 2024.10.17 @ 04:07 AM EST:
		- Stable:
			- automatic-ripping-machine: v2.8.1 --> v2.9.0
			- immich: v1.118.1 --> v1.118.2
			- ipfs: v0.30.0 --> v0.31.0
			- minio: v2024.10.02 --> v2024.10.13
			- mosquitto: v2.0.19 --> v2.0.20
			- nginx-proxy-manager: v2.12.0 --> v2.12.1
			- nocodb: v0.257.0 --> v0.257.2
			- sourcegraph: v5.8.0 --> v5.8.1579
			- tailscale: v1.74.1 --> v1.76.1
	- 2024.10.16 @ 03:49 PM EST:
		- Stable:
			- bookstack: v24.10.20241009 --> v24.10.20241014
			- chroma: v0.5.13 --> v0.5.15
			- esphome: v2024.9.2 --> v2024.10.0
			- fluidd: v1.30.4 --> v1.30.5
			- ghostfolio: v2.114.0 --> v2.115.0
			- homepage: v0.9.10 --> v0.9.11
			- immich: v1.117.0 --> v1.118.1
			- jackett: v0.22.800 --> v0.22.806
			- metabase: v0.50.29 --> v0.50.30
			- minecraft-java: v2024.5.0 --> v2024.10.1
			- n8n: v1.63.4 --> v1.64.0
			- nginx-proxy-manager: v2.11.3 --> v2.12.0
			- qbitrr: v4.9.10 --> v4.9.11
			- satisfactory: v1.8.7 --> v1.8.8
			- stash: v0.27.1 --> v0.27.2
			- syncthing: v1.27.12 --> v1.28.0
			- tauticord: v5.7.2 --> v5.7.3
			- watcharr: v1.44.1 --> v1.44.2
		- Incubator:
			- pingvin-share: v1.2.0 --> v1.2.1
	- 2024.10.15 @ 03:48 PM EST:
		- Stable:
			- healthchecks: v3.6.20241007 --> v3.6.20241014
			- jackett: v0.22.779 --> v0.22.800
			- jenkins: v2.480.0 --> v2.481.0
			- komga: v1.14.0 --> v1.14.1
			- misskey: v2024.10.0 --> v2024.10.1
			- mysql-workbench: v8.0.38 --> v8.0.40
			- n8n: v1.63.2 --> v1.63.4
			- portainer: v2.22.0 --> v2.23.0
			- radicale: v3.2.3.1 --> v3.3.0.0
			- shlink: v4.2.1 --> v4.2.2
			- ubooquity: v2.1.4 --> v2.1.5
			- watcharr: v1.44.0 --> v1.44.1
			- wyoming-whisper: v2.1.0 --> v2.2.0
			- zwavejs2mqtt: v9.22.0 --> v9.23.0
		- Incubator:
			- docuseal: v1.7.5 --> v1.7.6
			- pingvin-share: v1.1.3 --> v1.2.0
		- System:
			- volsync: v0.9.1 --> v0.10.0
		- Premium:
			- vaultwarden: v1.32.1 --> v1.32.2
	- 2024.10.15 @ 05:03 AM EST:
		- Stable:
			- audiobookshelf: v2.14.0 --> v2.15.0
			- jackett: v0.22.763 --> v0.22.779
			- local-ai: v2.21.1 --> v2.22.0
			- prowlarr: v1.25.1.4770 --> v1.25.2.4794
			- radarr: v5.11.0.9244 --> v5.12.2.9335
			- shoko-server: v4.2.2 --> v5.0.0
			- tautulli: v2.14.5 --> v2.14.6
			- twofauth: v5.3.0 --> v5.3.1
			- whisparr: v3.0.0.617 --> v3.0.0.621
			- wikijs: v2.5.304 --> v2.5.305
	- 2024.10.12 @ 07:14 AM EST:
		- Stable:
			- alist: v3.37.4 --> v3.38.0
			- changedetection-io: v0.46.04 --> v0.47.03
			- collabora: v24.04.8.1.1 --> v24.04.8.2.1
			- ddns-go: v6.7.0 --> v6.7.1
			- deconz: v2.28.1 --> v2.29.0
			- firefox: v130.0.1 --> v131.0.2
			- flexget: v3.11.46 --> v3.11.48
			- home-assistant: v2024.10.1 --> v2024.10.2
			- jackett: v0.22.756 --> v0.22.763
			- n8n: v1.63.1 --> v1.63.2
			- scrypted: v0.119.1 --> v0.119.2
			- unifi: v8.4.62 --> v8.5.6
			- vocechat-server: v0.3.54 --> v0.3.57
			- zwavejs2mqtt: v9.21.1 --> v9.22.0
	- 2024.10.11 @ 03:39 AM EST:
		- Stable:
			- chroma: v0.5.12 --> v0.5.13
			- cloudflared: v2024.9.1 --> v2024.10.0
			- flood: v4.8.3 --> v4.8.4
			- flowise: v2.1.1 --> v2.1.2
			- ghostfolio: v2.113.0 --> v2.114.0
			- jackett: v0.22.749 --> v0.22.756
			- metabase: v0.50.28 --> v0.50.29
			- mongodb: v8.0.0 --> v8.0.1
			- n8n: v1.62.3 --> v1.63.1
			- netdata: v1.47.3 --> v1.47.4
			- nexus-oss: v3.72.0 --> v3.73.0
			- nocodb: v0.256.0 --> v0.257.0
			- node-red: v4.0.4 --> v4.0.5
			- ollama: v0.3.12 --> v0.3.13
			- qbitrr: v4.9.7 --> v4.9.10
			- shlink-web-client: v4.2.0 --> v4.2.1
			- smtp-relay: v0.5.5 --> v0.5.6
			- speedtest-tracker: v0.21.2 --> v0.21.4
			- stash: v0.27.0 --> v0.27.1
			- whisparr: v3.0.0.614 --> v3.0.0.617
	- 2024.10.09 @ 01:02 PM EST:
		- Stable:
			- bookstack: v24.05.20240520 --> v24.10.20241009
			- chroma: v0.5.11 --> v0.5.12
			- ctfd: v3.7.3 --> v3.7.4
			- gitea: v1.22.2 --> v1.22.3
			- jackett: v0.22.735 --> v0.22.749
			- lidarr: v2.5.3.4341 --> v2.6.4.4402
			- misskey: v2024.9.0 --> v2024.10.0
			- nocodb: v0.255.2 --> v0.256.0
			- node-red: v4.0.3 --> v4.0.4
			- odoo: v17.0.0 --> v18.0.0
			- qbitrr: v4.9.6 --> v4.9.7
			- whisparr: v3.0.0.610 --> v3.0.0.614
	- 2024.10.08 @ 08:33 PM EST:
		- Stable:
			- mongodb: v7.0.14 --> v8.0.0
		- System:
			- snapshot-controller: v8.0.1 --> v8.1.0
	- 2024.10.08 @ 04:23 PM EST:
		- Stable:
			- actualserver: v24.10.0 --> v24.10.1
			- autobrr: v1.46.1 --> v1.47.1
			- flood: v4.8.2 --> v4.8.3
			- ghostfolio: v2.112.0 --> v2.113.0
			- healthchecks: v3.6.20240930 --> v3.6.20241007
			- ispy-agent-dvr: v5.7.9.0 --> v5.8.0.0
			- jackett: v0.22.714 --> v0.22.735
			- jenkins: v2.479.0 --> v2.480.0
			- metube: v2024.10.4 --> v2024.10.8
			- n8n: v1.62.1 --> v1.62.3
			- prowlarr: v1.25.0.4759 --> v1.25.1.4770
			- qbitmanage: v4.1.10 --> v4.1.11
			- shlink-web-client: v4.1.2 --> v4.2.0
			- sourcegraph: v5.7.2474 --> v5.8.0
			- tagspaces: v6.0.1 --> v6.0.2
			- tandoor-recipes: v1.5.19 --> v1.5.20
			- tasmobackup: v1.06.06 --> v1.06.09
			- watcharr: v1.43.0 --> v1.44.0
			- webgrabplus: v5.2.2 --> v5.3.0
		- Incubator:
			- docuseal: v1.7.4 --> v1.7.5
		- Premium:
			- authelia: v4.38.15 --> v4.38.16
	- 2024.10.07 @ 02:25 AM EST:
		- Stable:
			- prowlarr: v1.24.3.4754 --> v1.25.0.4759
	- 2024.10.06 @ 12:18 AM EST:
		- Stable:
			- audiobookshelf: v2.13.4 --> v2.14.0
			- baserow: v1.23.0 --> v1.28.0
			- homebox: v0.15.0 --> v0.15.2
			- jackett: v0.22.707 --> v0.22.714
			- shiori: v1.7.0 --> v1.7.1
			- slink: v1.1.0 --> v1.2.1
	- 2024.10.05 @ 07:15 AM EST:
		- Stable:
			- actualserver: v24.9.0 --> v24.10.0
			- adguard-home: v0.107.52 --> v0.107.53
			- bazarr: v1.4.4 --> v1.4.5
			- clickhouse: v24.9.1.3278 --> v24.9.2.42
			- collabora: v24.04.7.2.1 --> v24.04.8.1.1
			- crafty-4: v4.4.3 --> v4.4.4
			- dashdot: v5.8.6 --> v5.9.0
			- drawio: v24.7.8 --> v24.7.17
			- emby: v4.8.7.0 --> v4.9.0.30
			- esphome: v2024.9.1 --> v2024.9.2
			- filebrowser: v2.31.1 --> v2.31.2
			- fileflows: v24.09.0 --> v24.10.0
			- ghostfolio: v2.111.0 --> v2.112.0
			- gokapi: v1.9.1 --> v1.9.2
			- home-assistant: v2024.9.3 --> v2024.10.1
			- homebox: v0.14.2 --> v0.15.0
			- immich: v1.116.2 --> v1.117.0
			- jackett: v0.21.2831 --> v0.22.707
			- jenkins: v2.478.0 --> v2.479.0
			- kometa: v2.0.2 --> v2.1.0
			- lidarr: v2.5.2.4316 --> v2.5.3.4341
			- linkding: v1.35.0 --> v1.36.0
			- meshcentral: v1.1.31 --> v1.1.32
			- metabase: v0.50.27 --> v0.50.28
			- metube: v2024.9.28 --> v2024.10.4
			- minio: v2024.09.22 --> v2024.10.02
			- mosquitto: v2.0.18 --> v2.0.19
			- n8n: v1.61.0 --> v1.62.1
			- netdata: v1.47.2 --> v1.47.3
			- notifiarr: v0.8.2 --> v0.8.3
			- nzbget: v24.1.0 --> v24.3.0
			- nzbhydra: v7.1.0 --> v7.2.3
			- pinry: v2.1.12 --> v2.1.13
			- plexripper: v0.22.0 --> v0.23.2
			- portainer: v2.21.2 --> v2.22.0
			- qbitmanage: v4.1.9 --> v4.1.10
			- readarr: v0.3.32.2587 --> v0.4.0.2634
			- redis: v7.4.0 --> v7.4.1
			- redisinsight: v2.56.0 --> v2.58.0
			- shlink: v4.2.0 --> v4.2.1
			- tagspaces: v5.5.2 --> v6.0.1
			- tinymediamanager: v5.0.11 --> v5.0.12
			- traggo: v0.4.5 --> v0.5.0
			- whoogle: v0.8.4 --> v0.9.0
			- xen-orchestra: v5.156.0 --> v5.157.1
			- xwiki: v16.7.1 --> v16.8.0
			- youtubedl-material: v4.3.2 --> v2024.10.01
			- zerotier: v1.14.0 --> v1.14.1
			- zigbee2mqtt: v1.40.1 --> v1.40.2
			- zwavejs2mqtt: v9.21.0 --> v9.21.1
		- Incubator:
			- victoriametrics: v1.103.0 --> v1.104.0
		- Premium:
			- grafana: v11.2.1 --> v11.2.2
			- traefik: v3.1.4 --> v3.1.5
			- vaultwarden: v1.32.0 --> v1.32.1
	- 2024.09.30 @ 11:13 AM EST:
		- Stable:
			- avidemux: v24.07.1 --> v24.09.1
			- czkawka: v24.07.1 --> v24.09.1
			- filebot: v24.07.1 --> v24.09.1
			- healthchecks: v3.6.20240916 --> v3.6.20240930
			- jdownloader2: v24.08.1 --> v24.09.1
			- mediainfo: v24.08.1 --> v24.09.1
			- mkvcleaver: v24.07.1 --> v24.09.1
			- mkvtoolnix: v24.09.1 --> v24.09.2
			- openhab: v4.2.1 --> v4.2.2
			- plexripper: v0.21.0 --> v0.22.0
			- putty: v24.08.1 --> v24.09.1
			- qbittorrent: v4.6.7 --> v5.0.0
			- qdirstat: v24.07.2 --> v24.09.1
			- tsmuxer: v24.07.1 --> v24.09.1
			- uptime-kuma: v1.23.14 --> v1.23.15
		- Incubator:
			- docuseal: v1.7.3 --> v1.7.4
		- Premium:
			- authelia: v4.38.13 --> v4.38.15
	- 2024.09.29 @ 02:39 PM EST:
		- Stable:
			- fireflyiii: v6.1.20 --> v6.1.21
			- ghostfolio: v2.110.0 --> v2.111.0
			- misskey: v2024.8.0 --> v2024.9.0
			- plextraktsync: v0.31.13 --> v0.31.14
			- satisfactory: v1.8.6 --> v1.8.7
			- smtp-relay: v0.5.4 --> v0.5.5
			- uptime-kuma: v1.23.13 --> v1.23.14
			- vikunja: v0.24.3 --> v0.24.4
		- Premium:
			- authelia: v4.38.12 --> v4.38.13
	- 2024.09.28 @ 09:47 AM EST:
		- Stable:
			- adguardhome-sync: v0.6.12 --> v0.6.13
			- authentik: v2024.8.2 --> v2024.8.3
			- fireflyiii: v6.1.19 --> v6.1.20
			- immich: v1.116.0 --> v1.116.2
			- metube: v2024.9.26 --> v2024.9.28
			- miniflux: v2.2.0 --> v2.2.1
			- navidrome: v0.53.2 --> v0.53.3
			- twofauth: v5.2.0 --> v5.3.0
			- xen-orchestra: v5.154.0 --> v5.156.0
			- zwavejs2mqtt: v9.20.0 --> v9.21.0
		- Incubator:
			- pingvin-share: v1.1.2 --> v1.1.3
	- 2024.09.27 @ 01:19 PM EST:
		- Stable:
			- calibre: v7.18.0 --> v7.19.0
			- chroma: v0.5.9 --> v0.5.11
			- komga: v1.13.0 --> v1.14.0
			- meshcentral: v1.1.30 --> v1.1.31
			- prowlarr: v1.24.1.4740 --> v1.24.3.4754
			- qbitrr: v4.9.4 --> v4.9.6
	- 2024.09.26 @ 09:35 PM EST:
		- Stable:
			- borg-server: v2.6.3 --> v2.6.4
			- chroma: v0.5.7 --> v0.5.9
			- clickhouse: v24.8.4.13 --> v24.9.1.3278
			- code-server: v4.92.2 --> v4.93.1
			- esphome: v2024.9.0 --> v2024.9.1
			- firefox: v128.0.3 --> v130.0.1
			- ghostfolio: v2.108.0 --> v2.110.0
			- gravity: v0.9.0 --> v0.9.1
			- home-assistant: v2024.9.2 --> v2024.9.3
			- homepage: v0.9.9 --> v0.9.10
			- immich: v1.115.0 --> v1.116.0
			- ispy-agent-dvr: v5.7.8.0 --> v5.7.9.0
			- jenkins: v2.477.0 --> v2.478.0
			- kanboard: v1.2.39 --> v1.2.40
			- linkding: v1.34.0 --> v1.35.0
			- local-ai: v2.20.1 --> v2.21.1
			- matomo: v5.1.1 --> v5.1.2
			- metabase: v0.50.26 --> v0.50.27
			- metube: v2024.9.16 --> v2024.9.26
			- minio: v2024.09.13 --> v2024.09.22
			- n8n: v1.60.1 --> v1.61.0
			- navidrome: v0.53.1 --> v0.53.2
			- netdata: v1.47.1 --> v1.47.2
			- notifiarr: v0.8.1 --> v0.8.2
			- ollama: v0.3.11 --> v0.3.12
			- outline: v0.79.1 --> v0.80.2
			- pgadmin: v8.11.0 --> v8.12.0
			- plex: v1.41.0.8992 --> v1.41.0.8994
			- pocketmine-mp: v5.18.1 --> v5.19.0
			- portainer: v2.21.1 --> v2.21.2
			- prowlarr: v1.24.0.4721 --> v1.24.1.4740
			- qbitrr: v4.9.3 --> v4.9.4
			- radarr: v5.9.1.9070 --> v5.11.0.9244
			- stash: v0.26.2 --> v0.27.0
			- tautulli: v2.14.4 --> v2.14.5
			- tdarr: v2.25.01 --> v2.26.01
			- tdarr-node: v2.25.01 --> v2.26.01
			- vocechat-server: v0.3.50 --> v0.3.54
			- wekan: v7.59.0 --> v7.60.0
			- zwavejs2mqtt: v9.19.0 --> v9.20.0
		- Incubator:
			- docuseal: v1.7.2 --> v1.7.3
			- pingvin-share: v1.1.1 --> v1.1.2
		- Premium:
			- authelia: v4.38.11 --> v4.38.12
			- grafana: v11.2.0 --> v11.2.1
			- traefik: v3.1.3 --> v3.1.4
	- 2024.09.21 @ 08:18 PM EST:
		- Premium:
			- nextcloud: v29.0.7 --> v30.0.0
	- 2024.09.21 @ 07:26 AM EST:
		- Stable:
			- ddns-updater: v2.8.0 --> v2.8.1
			- docker: v27.2.1 --> v27.3.1
			- ersatztv: v0.8.7 --> v0.8.8
			- flexget: v3.11.45 --> v3.11.46
			- ispy-agent-dvr: v5.7.6.0 --> v5.7.8.0
			- n8n: v1.60.0 --> v1.60.1
			- satisfactory: v1.8.5 --> v1.8.6
			- tauticord: v5.7.1 --> v5.7.2
			- vikunja: v0.24.2 --> v0.24.3
		- Premium:
			- authelia: v4.38.10 --> v4.38.11
			- nextcloud: v29.0.6 --> v29.0.7
	- 2024.09.19 @ 12:02 AM EST:
		- Stable:
			- alist: v3.37.3 --> v3.37.4
			- chroma: v0.5.5 --> v0.5.7
			- esphome: v2024.8.3 --> v2024.9.0
			- flowise: v2.1.0 --> v2.1.1
			- kavita: v0.8.2 --> v0.8.3
			- n8n: v1.59.2 --> v1.60.0
			- ollama: v0.3.10 --> v0.3.11
			- radicale: v3.2.3.0 --> v3.2.3.1
			- sourcegraph: v5.7.0 --> v5.7.2474
			- tailscale: v1.72.1 --> v1.74.1
			- traccar: v6.4.0 --> v6.5.0
			- wikijs: v2.5.303 --> v2.5.304
		- Incubator:
			- pingvin-share: v1.1.0 --> v1.1.1
	- 2024.09.17 @ 11:56 PM EST:
		- Stable:
			- ddns-updater: v2.7.1 --> v2.8.0
			- flowise: v2.0.7 --> v2.1.0
			- ghostfolio: v2.107.1 --> v2.108.0
			- jenkins: v2.476.0 --> v2.477.0
			- metabase: v0.50.25 --> v0.50.26
			- n8n: v1.59.1 --> v1.59.2
			- navidrome: v0.53.0 --> v0.53.1
			- node-red: v4.0.2 --> v4.0.3
			- static-web-server: v2.32.2 --> v2.33.0
			- watchyourlan: v2.0.2 --> v2.0.3
	- 2024.09.17 @ 08:03 PM EST:
		- Stable:
			- ddns-updater: v2.7.0 --> v2.7.1
			- game-server-watcher: v3.1.18 --> v3.1.20
			- navidrome: v0.52.5 --> v0.53.0
			- openvscode-server: v1.93.0 --> v1.93.1
			- qbittorrent: v4.6.6 --> v4.6.7
			- zwavejs2mqtt: v9.18.1 --> v9.19.0
		- Premium:
			- traefik: v3.1.2 --> v3.1.3
	- 2024.09.16 @ 06:41 PM EST:
		- Incubator:
			- docuseal: v1.7.1 --> v1.7.2
		- Stable:
			- alist: v3.37.2 --> v3.37.3
			- authentik: v2024.8.1 --> v2024.8.2
			- healthchecks: v3.6.20240909 --> v3.6.20240916
			- home-assistant: v2024.9.1 --> v2024.9.2
			- linkding: v1.33.0 --> v1.34.0
			- metube: v2024.9.11 --> v2024.9.16
			- n8n: v1.59.0 --> v1.59.1
			- paperless-ngx: v2.12.0 --> v2.12.1
			- photoprism: v240711.0.0 --> v240915.0.0
			- splunk: v9.3.0 --> v9.3.1
			- theme-park: v1.17.0 --> v1.18.0
	- 2024.09.15 @ 10:40 PM EST:
		- Stable:
			- bazarr: v1.4.3 --> v1.4.4
			- minetest: v5.9.0 --> v5.9.1
			- requestrr: v2.1.6 --> v2.1.7
			- ubooquity: v2.1.2 --> v2.1.4
	- 2024.09.15 @ 07:30 PM EST:
		- Stable:
			- meshcentral: v1.1.29 --> v1.1.30
	- 2024.09.15 @ 12:42 PM EST:
		- Incubator:
			- pingvin-share: v1.0.4 --> v1.1.0
			- slskd: v0.21.3 --> v0.21.4
		- Stable:
			- cops: v3.1.3 --> v3.2.2
			- handbrake: v24.06.1 --> v24.09.1
			- homebox: v0.14.1 --> v0.14.2
			- minio: v2024.09.09 --> v2024.09.13
			- recyclarr: v7.2.3 --> v7.2.4
			- satisfactory: v1.8.4 --> v1.8.5
			- tdarr-node: v2.24.05 --> v2.25.01
			- tdarr: v2.24.05 --> v2.25.01
	- 2024.09.14 @ 11:09 AM EST:
		- Stable:
			- impostor-server: v1.9.3 --> v1.10.0
			- linkding: v1.32.0 --> v1.33.0
			- xen-orchestra: v5.153.1 --> v5.154.0
	- 2024.09.13 @ 10:26 PM EST:
		- Stable:
			- flexget: v3.11.43 --> v3.11.45
	- 2024.09.13 @ 06:20 PM EST:
		- Stable:
			- alist: v3.37.1 --> v3.37.2
			- collabora: v24.04.7.1.2 --> v24.04.7.2.1
			- mkvtoolnix: v24.07.2 --> v24.09.1
			- qinglong: v2.17.10 --> v2.17.11
			- scrypted: v0.119.0 --> v0.119.1
	- 2024.09.13 @ 11:18 AM EST:
		- Stable:
			- maintainerr: v2.1.1 --> v2.1.2
			- satisfactory: v1.8.3 --> v1.8.4
	- 2024.09.13 @ 03:39 AM EST:
		- Stable:
			- automatic-ripping-machine: v2.8.0 --> v2.8.1
			- calibre: v7.17.0 --> v7.18.0
			- ghostfolio: v2.107.0 --> v2.107.1
			- synclounge: v5.2.31 --> v5.2.33
	- 2024.09.12 @ 08:19 PM EST:
		- Stable:
			- autobrr: v1.46.0 --> v1.46.1
			- cops: v3.1.2 --> v3.1.3
			- emulatorjs: v1.9.0 --> v1.9.2
			- immich: v1.114.0 --> v1.115.0
			- satisfactory: v1.8.1 --> v1.8.3
	- 2024.09.12 @ 10:08 AM EST:
		- Stable:
			- autobrr: v1.45.0 --> v1.46.0
			- fluidd: v1.30.3 --> v1.30.4
			- plex: v1.40.5.8921 --> v1.41.0.8992
			- qbitrr: v4.9.2 --> v4.9.3
			- satisfactory: v1.7.4 --> v1.8.1
	- 2024.09.11 @ 09:23 PM EST:
		- Stable:
			- unifi: v8.4.59 --> v8.4.62
	- 2024.09.11 @ 04:18 PM EST:
		- Stable:
			- ipfs: v0.29.0 --> v0.30.0
			- ispy-agent-dvr: v5.7.5.0 --> v5.7.6.0
			- komga: v1.12.1 --> v1.13.0
			- metube: v2024.8.22 --> v2024.9.11
			- n8n: v1.58.1 --> v1.59.0
			- satisfactory: v1.7.3 --> v1.7.4
			- wordpress: v6.6.1 --> v6.6.2
	- 2024.09.11 @ 01:57 AM EST:
		- Incubator:
			- docuseal: v1.5.6 --> v1.7.1
			- pingvin-share: v0.24.1 --> v1.0.4
			- semaphore: v2.9.75 --> v2.19.10
			- slskd: v0.20.1 --> v0.21.3
			- teslamate: v1.29.1 --> v1.30.1
			- victoriametrics: v1.99.0 --> v1.103.0
		- Premium:
			- grafana: v11.0.0 --> v11.2.0
			- prometheus: v2.52.0 --> v2.54.1
			- vaultwarden: v1.30.5 --> v1.32.0
		- Stable:
			- ghostfolio: v2.106.0 --> v2.107.0
			- linkding: v1.31.1 --> v1.32.0
			- metabase: v0.50.24 --> v0.50.25
			- satisfactory: v1.7.1 --> v1.7.3
			- scrypted: v0.118.0 --> v0.119.0
		- System:
			- snapshot-controller: v7.0.1 --> v8.0.1
	- 2024.09.10 @ 07:17 PM EST:
		- Stable:
			- audiobookshelf: v2.13.3 --> v2.13.4
			- cloudflared: v2024.8.3 --> v2024.9.1
			- cops: v2.8.1 --> v3.1.2
			- docker: v27.2.0 --> v27.2.1
			- homepage: v0.9.6 --> v0.9.9
			- jenkins: v2.475.0 --> v2.476.0
			- minio: v2024.08.29 --> v2024.09.09
			- netdata: v1.47.0 --> v1.47.1
			- portainer: v2.21.0 --> v2.21.1
			- redisinsight: v2.54.0 --> v2.56.0
			- satisfactory: v1.6.2 --> v1.7.1
			- solr: v9.6.1 --> v9.7.0
	- 2024.09.09 @ 05:53 PM EST:
		- Stable:
			- alist: v3.36.0 --> v3.37.1
			- authentik: v2024.8.0 --> v2024.8.1
			- game-server-watcher: v3.1.17 --> v3.1.18
			- ghostfolio: v2.105.0 --> v2.106.0
			- healthchecks: v3.6.20240904 --> v3.6.20240909
			- ispy-agent-dvr: v5.7.4.0 --> v5.7.5.0
			- jellyfin: v10.9.10 --> v10.9.11
			- maintainerr: v2.1.0 --> v2.1.1
			- memcached: v1.6.30 --> v1.6.31
			- meshcentral: v1.1.27 --> v1.1.29
			- ollama: v0.3.9 --> v0.3.10
			- paperless-ngx: v2.11.6 --> v2.12.0
			- plextraktsync: v0.31.12 --> v0.31.13
			- prowlarr: v1.23.1.4708 --> v1.24.0.4721
			- scrypted: v0.117.3 --> v0.118.0
			- tinymediamanager: v5.0.10 --> v5.0.11
			- watchyourlan: v2.0.1 --> v2.0.2
			- whisparr: v3.0.0.607 --> v3.0.0.610
			- zigbee2mqtt: v1.40.0 --> v1.40.1
	- 2024.09.08:
   		- Updated all apps to match truecharts versions. You can check the commmits for the full list
