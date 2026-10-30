<h1 align="center">Kinetic</h1>

<p align="center">
  A visual progression path for learning calisthenics.
</p>

<p align="center">
  <strong>Harel Meltser · Co-founder &amp; CTO</strong><br />
  Native iOS · <a href="https://apps.apple.com/us/app/kinetic-calisthenics-training/id6766755091">Live on the App Store</a>
</p>

Kinetic helps people discover calisthenics skills, understand their prerequisites, and track progress through an interactive skill tree.

<table>
  <tr>
    <th align="center">Progression tree</th>
    <th align="center">Skill progression</th>
  </tr>
  <tr>
    <td align="center">
      <a href="assets/tree-overview.png">
        <img src="assets/tree-overview.png" width="300" alt="Kinetic's zoomed-out progression tree showing connected calisthenics skills and rank badges." />
      </a>
    </td>
    <td align="center">
      <a href="assets/skill-detail.png">
        <img src="assets/skill-detail.png" width="300" alt="A close-up of Kinetic's planche progression, with ranks, logged repetitions, and hold times." />
      </a>
    </td>
  </tr>
  <tr>
    <td align="center">Connected skills and prerequisites.</td>
    <td align="center">Ranks and logged performance.</td>
  </tr>
</table>

## What I built

- **Native iOS rebuild.** Proposed and led the move from React Native to native iOS, building the SwiftUI interface and SpriteKit skill tree.
- **Progression logic.** Built the system that maps logged repetitions and hold times to ranks, tracks progress toward the next threshold, and unlocks skills when prerequisites are met.
- **Accounts and subscriptions.** Built and integrated account and progress storage, subscription access, purchase restoration, and product analytics.

## Engineering the tree

The tree is an interactive interface, not a static diagram. SwiftUI handles the surrounding screens, while a retained SpriteKit scene handles the graph and its camera interactions. The scene reuses nodes, adjusts visual detail with zoom, and updates individual skill states without rebuilding the entire graph for each change.

**Built with:** Swift · SwiftUI · SpriteKit · Supabase · RevenueCat · PostHog

## Collaboration

I co-founded Kinetic with [Ilay Gibor](https://github.com/ilaygibor), who leads calisthenics content and growth and also contributes to product and engineering. This page focuses on my engineering responsibilities within our shared work.

The production source code is private. This repository is a public product and engineering overview.
