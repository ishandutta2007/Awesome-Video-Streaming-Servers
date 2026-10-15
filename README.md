# Awesome-Video-Streaming-Servers

# Top Video Streaming Servers Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Live Ingest, RTMP/SRT/WebRTC, HLS/DASH Packaging, Media Servers & Broadcast Origin*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Video Streaming Servers**. These systems ingest live video, transcode or package it, and deliver streams via RTMP, SRT, WebRTC, HLS, DASH, and related protocols.

**Examples** include Wowza, Red5 Pro, Ant Media Server, Nimble Streamer, Flussonic, AWS Elemental MediaLive, Azure Media Services, Cloudflare Stream, Vimeo Enterprise, Dacast, and **nginx-rtmp** (`arut/nginx-rtmp-module`)—NGINX-based media streaming server module.

**Open-source emphasis**: Live media servers are strong in open source. **MediaMTX**, **SRS**, **nginx-rtmp**, **Owncast**, and **Ant Media** (community) cover ingest-to-playback pipelines. This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[AWS Elemental MediaLive / MediaPackage, Azure Media Services, Cloudflare Stream](https://aws.amazon.com/medialive/)**  
  Cloud live and on-demand media pipelines—managed encoding, packaging, and global delivery.

- **[Wowza, Red5 Pro, Ant Media (enterprise), Flussonic, Nimble](https://www.wowza.com/)**  
  Dedicated media server products—low-latency streaming, WebRTC, and professional broadcast features.

- **[Vimeo Enterprise, Dacast, other OVP live offerings](https://vimeo.com/)**  
  Online video platforms with live streaming, player, and monetization layers.

- **[Other commercial streaming platforms](https://www.cloudflare.com/products/cloudflare-stream/)**  
  Additional CDN-integrated and turnkey live services.

## Open-Source GitHub Projects

### Live Media Servers

- **[MediaMTX](https://github.com/bluenviron/mediamtx)**  
  Ready-to-use open live media server and proxy—RTMP, RTSP, WebRTC, SRT, HLS, and more; single binary, hot reload, recording, and protocol conversion.

- **[SRS (Simple Realtime Server)](https://github.com/ossrs/srs)**  
  Open high-performance streaming server—RTMP, WebRTC, SRT, HLS, HTTP-FLV; strong for large-scale and clustered live setups.

- **[nginx-rtmp-module](https://github.com/arut/nginx-rtmp-module)**  
  Classic NGINX-based RTMP/HLS streaming module—still widely deployed for simple ingest and relay (maintenance less active than newer servers).

- **[Owncast](https://github.com/owncast/owncast)**  
  Open self-hosted live streaming and chat platform—Twitch-style experience you run yourself.

- **[Ant Media Server (Community)](https://github.com/ant-media/Ant-Media-Server)**  
  Open media server with WebRTC and ultra-low-latency options; commercial edition available.

- **[Red5 (open / community lineage)](https://github.com/Red5)**  
  Open media server projects in the Red5 family for RTMP and real-time streaming.

### Tooling & Adjacent Stack

- **[FFmpeg](https://github.com/FFmpeg/FFmpeg)**  
  Essential open transcoder and packaging tool—used with every media server for ABR ladders and format conversion.

- **[OBS Studio](https://github.com/obsproject/obs-studio)**  
  Open broadcaster software—primary ingest client for RTMP/SRT to media servers.

- **[Janus / LiveKit (WebRTC selective forwarding)](https://github.com/meetecho/janus-gateway)**  
  Open WebRTC SFUs often paired with streaming workflows for interactive ultra-low latency.

- **[PeerTube](https://github.com/Chocobozzz/PeerTube)**  
  Open ActivityPub video platform—federation-oriented hosting rather than pure live origin, useful for VOD + live communities.

- **[Jellyfin](https://github.com/jellyfin/jellyfin)**  
  Open media system focused on personal streaming libraries (VOD), complementary to live servers.

### Additional Strong Open-Source Options

- **General live origin / proxy**: MediaMTX.
- **Scale / cluster live**: SRS.
- **NGINX environments**: nginx-rtmp (legacy but common).
- **Creator self-host**: Owncast.
- **Composable stacks**: OBS → MediaMTX/SRS → FFmpeg ABR → CDN (Cloudflare/CloudFront) → player.
- Commercial platforms still lead for managed global packaging, SLA-backed transcoding, and turnkey monetization.

**Frameworks for building custom systems**:  
**MediaMTX** for simple multi-protocol routing; **SRS** for high-scale live; **Owncast** for community streaming sites; **FFmpeg** everywhere for encode/package.  
Fully open live streaming origins are production-ready; global last-mile delivery often still uses commercial CDNs.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS/hosted or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Live streaming can incur high bandwidth and legal liability (content rights, DMCA, local broadcast rules). Secure publish endpoints (keys, IP allowlists), monitor abuse, and size origin capacity for concurrent viewers.
- Open-source media servers offer control and cost efficiency. Commercial platforms shift encoding and global delivery to the vendor. Neither replaces content licensing and player accessibility requirements.

---

**Made for streaming engineers, broadcasters, and teams running their own live origins.**  
Let's expand open media servers while recognizing the global scale and packaging depth that leading commercial streaming platforms deliver.
