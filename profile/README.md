<div align="center">

<img src="https://avatars.githubusercontent.com/u/284947552?s=200&v=4" width="120" alt="Scoova" />

# Scoova

### Maps & Observability for apps that move people

One API key for routing, maps, geocoding, weather, storage, static images,
elevation, geofences, and webhooks &mdash; plus crash reporting, custom
events, and performance traces. Same SDKs, same dashboard, same support
inbox.

<p>
  <a href="https://scoo-va.info"><img src="https://img.shields.io/badge/scoo--va.info-0F172A?style=for-the-badge&logoColor=white" alt="Website" /></a>
  <a href="https://monitor.scoo-va.info"><img src="https://img.shields.io/badge/dashboard-1E293B?style=for-the-badge&logoColor=white" alt="Dashboard" /></a>
  <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/badge/license-Apache_2.0-475569?style=for-the-badge" alt="Apache 2.0" /></a>
</p>

</div>

---

## Two products, one stack

### <picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/Scoova_Cloud-0EA5E9?style=for-the-badge&logoColor=white"><img src="https://img.shields.io/badge/Scoova_Cloud-0284C7?style=for-the-badge&logoColor=white" alt="Scoova Cloud"></picture>

The developer platform underneath every app that moves people.

| Service | What it does |
|---|---|
| **Routing** | Turn-by-turn navigation, custom costing, elevation-aware. Eyes-on-the-road voice cues that name landmarks &mdash; never streets &mdash; in eyes-off mode. |
| **Maps** | Five purpose-tuned styles (light, dark, drive, micromobility, satellite). Drop-in for MapLibre across every platform. Bike lanes drawn as bike lanes. |
| **Geocoding** | Forward, reverse, autocomplete, and a batch endpoint that resolves up to 100 addresses or coordinates in a single round-trip. |
| **Weather** | Current conditions, hourly outlook, seven-day forecast. Plain language, not weather codes. |
| **Storage** | Document store for the always-syncing data a mobility app needs &mdash; trip history, saved places, rider profiles, fleet state. Offline-first SDKs. |
| **Static Maps** | Edge-cached map renders for share cards, push notifications, and embeds. |
| **Elevation** | Height samples for any point or route shape. Powers slope-aware routing, climb-effort UX, and accurate energy estimates. |
| **Geofences** | Define GeoJSON polygons on the server, then ask in one call which ones contain a given lat/lon. Server-side ray-cast. |
| **Webhooks** | HMAC-SHA256 signed payloads with `X-Scoova-Signature` header. |

### <picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/Scoova_Monitor-10B981?style=for-the-badge&logoColor=white"><img src="https://img.shields.io/badge/Scoova_Monitor-059669?style=for-the-badge&logoColor=white" alt="Scoova Monitor"></picture>

The observability stack on top.

- **Crash reports with full symbolication** &mdash; iOS dSYMs, Android ProGuard, Flutter obfuscated traces, Web source maps, React Native both layers
- **Custom event tracking** &mdash; sign-ups, ride starts, payment completed, anything your app counts
- **Performance traces** &mdash; cold-start, frame rate, memory, network
- **Per-user activity timelines** &mdash; reconstruct what a user did before they hit a crash
- **App-store rating intel** &mdash; per-country breakdowns, review-sentiment, version-over-version
- **AI-powered fix suggestions** &mdash; symbolicated stack &rarr; specific code change

---

## Five SDKs, same shape

<p>
  <img src="https://img.shields.io/badge/iOS-000000?style=flat-square&logo=apple&logoColor=white" alt="iOS" />
  <img src="https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white" alt="Android" />
  <img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white" alt="Flutter" />
  <img src="https://img.shields.io/badge/React_Native-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React Native" />
  <img src="https://img.shields.io/badge/Web-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="Web" />
</p>

Same namespaces across every platform. Same one API key authenticates against
both products.

| Platform | Monitor | Cloud | Distribution |
|---|---|---|---|
| **iOS** | <a href="https://cocoapods.org/pods/ScoovaMonitor"><img src="https://img.shields.io/badge/live-22C55E?style=flat-square" alt="ScoovaMonitor on CocoaPods" /></a> | <a href="https://cloud.scoo-va.info/docs"><img src="https://img.shields.io/badge/preview-F59E0B?style=flat-square" alt="Cloud preview docs" /></a> | Swift Package + CocoaPods |
| **Android** | <a href="https://central.sonatype.com/artifact/info.scoo-va/scoova-monitor-android"><img src="https://img.shields.io/badge/live-22C55E?style=flat-square" alt="scoova-monitor-android on Maven Central" /></a> | <a href="https://cloud.scoo-va.info/docs"><img src="https://img.shields.io/badge/preview-F59E0B?style=flat-square" alt="Cloud preview docs" /></a> | Maven Central (`info.scoo-va`) |
| **Flutter** | <a href="https://pub.dev/packages/scoova_monitor"><img src="https://img.shields.io/badge/live-22C55E?style=flat-square" alt="scoova_monitor on pub.dev" /></a> | <a href="https://cloud.scoo-va.info/docs"><img src="https://img.shields.io/badge/preview-F59E0B?style=flat-square" alt="Cloud preview docs" /></a> | pub.dev (verified publisher) |
| **React Native** | <a href="https://www.npmjs.com/package/@scoova/monitor-react-native"><img src="https://img.shields.io/badge/live-22C55E?style=flat-square" alt="@scoova/monitor-react-native on npm" /></a> | <a href="https://cloud.scoo-va.info/docs"><img src="https://img.shields.io/badge/preview-F59E0B?style=flat-square" alt="Cloud preview docs" /></a> | npm (`@scoova/*`) trusted publisher |
| **Web** | <a href="https://www.npmjs.com/package/@scoova/monitor-web"><img src="https://img.shields.io/badge/live-22C55E?style=flat-square" alt="@scoova/monitor-web on npm" /></a> | <a href="https://cloud.scoo-va.info/docs"><img src="https://img.shields.io/badge/preview-F59E0B?style=flat-square" alt="Cloud preview docs" /></a> | npm + jsDelivr CDN |

---

## Quick install

<details>
<summary><strong>iOS &mdash; Swift Package Manager</strong></summary>

```swift
dependencies: [
    .package(url: "https://github.com/Scoova/scoova-monitor-ios", from: "1.5.1")
]
```

Or via CocoaPods:

```ruby
pod 'ScoovaMonitor', '~> 1.5.1'
```
</details>

<details>
<summary><strong>Android &mdash; Gradle (Maven Central)</strong></summary>

```kotlin
dependencies {
    implementation("info.scoo-va:scoova-monitor-android:1.5.1")
}
```
</details>

<details>
<summary><strong>Flutter &mdash; pub.dev</strong></summary>

```yaml
dependencies:
  scoova_monitor: ^1.5.2
```
</details>

<details>
<summary><strong>React Native &mdash; npm</strong></summary>

```bash
npm install @scoova/monitor-react-native
```
</details>

<details>
<summary><strong>Web &mdash; npm or CDN</strong></summary>

```bash
npm install @scoova/monitor-web
```

Or drop the CDN tag straight into your `<head>`:

```html
<script src="https://cdn.jsdelivr.net/npm/@scoova/monitor-web@1.5.0/dist/monitor.js"></script>
```
</details>

---

## Why we built this

Every ride-hail, delivery, scooter-sharing, and fleet-ops platform needs the
same stack: maps, routing, geocoding, trip events, observability. Today they
assemble it from a dozen vendors. We bundled it under one API key, one
namespace, one dashboard.

Every product decision is filtered through one question:
**will the rider have to look down?** If yes, we redesign. Voice cues name
landmarks, not streets. The phone never has to leave the mount.

---

## Engineering

<p>
  <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" alt="Kotlin" />
  <img src="https://img.shields.io/badge/Swift-F05138?style=flat-square&logo=swift&logoColor=white" alt="Swift" />
  <img src="https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white" alt="Dart" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white" alt="Nginx" />
  <img src="https://img.shields.io/badge/Gradle-02303A?style=flat-square&logo=gradle&logoColor=white" alt="Gradle" />
  <img src="https://img.shields.io/badge/SwiftPM-F05138?style=flat-square&logo=swift&logoColor=white" alt="SwiftPM" />
  <img src="https://img.shields.io/badge/CocoaPods-EE3322?style=flat-square&logo=cocoapods&logoColor=white" alt="CocoaPods" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions" />
</p>

Every SDK ships via CI on a verified-publisher pipeline &mdash; pub.dev OIDC
trust, npm trusted publishers with SLSA provenance, Sonatype Central
Portal with in-memory PGP signing, CocoaPods trunk on tag. Zero
long-lived secrets across four of the five distribution channels.

The full stack &mdash;  45 native SDKs, navigation engine,
verified-publisher release pipelines, dashboard, AI symbolication &mdash; is
built and maintained by a small team led by
[**Mohammed Zaid**](https://github.com/zaidzedoo007) · [LinkedIn](https://www.linkedin.com/in/mohammed-zaid-6860a1237/) · [Scoova on LinkedIn](https://www.linkedin.com/company/scoova/). Reach out for
platform / SDK / DevTools engineering work:
[zaid@scoo-va.info](mailto:zaid@scoo-va.info).

---

<div align="center">

<sub>
Built with conviction for mobility, not advertising. &middot;
<a href="https://scoo-va.info">scoo-va.info</a> &middot;
<a href="https://monitor.scoo-va.info">monitor.scoo-va.info</a> &middot;
<a href="mailto:zaid@scoo-va.info">zaid@scoo-va.info</a>
</sub>

</div>
