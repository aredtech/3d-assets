# 3D Assets

GLB assets hosted for WebSDK applications.

## jsDelivr

Use a tagged release for stable URLs:

```text
https://cdn.jsdelivr.net/gh/aredtech/3d-assets@v2.2.0/<asset>.glb
```

Example:

```text
https://cdn.jsdelivr.net/gh/aredtech/3d-assets@v2.2.0/hos-017.glb
```

`manifest.json` describes all 329 assets. Pre-baked thumbnails are available as
`<asset-id>.webp` in the same release root.

## Catalog

Since `v2.0.0` the catalog holds the "Facility Props" set — 245 props, rooms,
and complete facilities in real-world meters, Y-up — plus `cctv-ptz-camera`.
Ids are the facility code lowercased (`SCH-001` → `sch-001`); each facility is
one manifest category: `school`, `hospital`, `airport`, `prison`, `mall`,
`office`, `industry`, `structural`, plus `cameras` for the surveillance
cameras. Since `v2.0.1` every model is centred on its footprint and merges its
static parts into one mesh per material.

Since `v2.1.0` the catalog adds the `events` category, the "Event Kit":
twelve trade-show and venue models (`evt-001`…`evt-012`: booth, backdrop
wall, hanging and blade banners, roll-up banner, teardrop flag, counter, LED
wall, cocktail tables, lectern, stage with truss, brochure rack), built to
the same conventions. Eight declare `metadata.signFaces`, where the WebSDK's
3D+ view writes a FeatureModel element's `sign:text`.

Since `v2.2.0` the catalog adds five generated kits, built in code to the
same conventions: Building Essentials (`amenities`, `ame-001`…`ame-021`:
washrooms, fire and first-aid points, exit and assembly signs, planters, a
water cooler, an ATM, coat and umbrella stands, waste sorting), the
Hospitality Kit (`hospitality`, `hsp-001`…`hsp-016`: hotel room and
furniture, café, restaurant, and bar counters, a commercial kitchen line),
the Parking Kit (`parking`, `prk-001`…`prk-010`: cars, a van, an EV
charger, barrier gates, a pay station, bay markings, a bike rack, a
guidance sign), the Tracking Kit (`tracking`, `trk-001`…`trk-016`: beacons,
anchors, gateways, an access point, an RFID portal, people, and tracked
equipment such as an AMR, a reach truck, and a stretcher), and the
Logistics Kit (`industry`, `lgx-001`…`lgx-008`: roll cages, a loading dock,
a parcel sorter, shelving, pallets, a packing station). Four of them
declare `metadata.signFaces`. Every `v2.1.0` file is unchanged.

Earlier releases (`v1.0.0`, `v1.0.2`, `v2.0.0`, `v2.0.1`, `v2.1.0`) stay available under their
immutable tags for clients pinned to them.

## Rights

The Facility Props models, the Event Kit, the generated kits, and `cctv-ptz-camera` were produced
for the Combain WebSDK. Assets in earlier tagged releases keep the rights of their respective
owners; public hosting does not grant permission to reuse or redistribute them
outside their licensed use.
