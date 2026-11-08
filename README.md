# Trackcress 1.0 TEST
Native Android Train Tracks railway puzzle. Android 8+ (min26), target35. Package com.gg007.trackcress. Twelve original uniquely solved 4x4 railway layouts.

## Rules
Train Tracks puzzle. Start at A on the left edge and tap orthogonal neighbors to extend the cyan tip towards B on the bottom edge. Use each visited cell once, with no crossing, branching or loop. Empty cells are allowed. Each top and right total counts occupied track cells in that column or row, including both A and B. Displayed values are current/target. Every gold rail cell must be visited with exactly its given two sides, including the external entry and exit sides at A and B. Gold shapes do not rotate. Side-neighboring track cells connect only when a rail is drawn between them; mere contact is allowed. CHECK confirms the completed A-to-B route, all eight totals and all gold shapes. Twelve original uniquely solved 4x4 layouts, each with three gold rail cells. Sequential route tapping is a control adaptation of standard Tracks edge drawing; fragments cannot be drawn separately. Unlimited undo/reset, next and level selection. Saved palette and optional a-p cell guides. No X pencil-mark mode in this edition.

## Download and status
https://mega.co.nz/#!BA8gTAaT!drjj-6MmEg7GoIEJ4_wbGxUZNRJCCRNvNTxqw35fF_A
APK SHA256 2b820785199d796e8b6d58e83be3b4916f4f40892709c94138e05930cfdcddda; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
An independent coordinate-graph oracle checks external endpoints, per-cell degree, required rail sides and row/column occupied-cell totals across all 10,974 simple-path prefixes from the twelve starts, stopping at B. It agrees with the production direction-mask validator and proves exactly one complete route on each board. All 256 ordered cell-pair adjacency cases pass, including diagonal and row-wrap rejection. Bounds, duplicate cells, early check, undo, solved lock, reset and route replay pass. The archived portable generator reproduces levels and the archived Java oracle reruns with byte-equal source. Actual drawing-adapter touch extension, solve/undo/replay, menu, levels, privacy and saved palette/cell guides pass. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 174 prior studio mechanics and all 803 web registry records. Railcress places cars with clues counting their empty sliding range; Trackcress draws one railway matching row/column occupancy totals and fixed rail shapes. Cindertrail collects sparks on a nonrepeating route without these line totals or rail-shape clues. Ribbonmere draws two separate paths covering every cell; Trackcress has one path and may leave cells empty. No Train Tracks functional match found in the reviewed catalog. Known Tracks adaptation, not a global invention claim. Original generated layouts, implementation and visuals; no source puzzle boards, code or art copied. Recovered repository corpus remains partial.
Rules https://www.chiark.greenend.org.uk/~sgtatham/puzzles/doc/tracks.html ; independent rules https://milomarwick.com/train-tracks/how-to-play .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/track-test src/com/gg007/trackcress/Board.java BoardTest.java then java -cp /tmp/track-test com.gg007.trackcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Trackcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, cell guides and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 175-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/ost5n0odd8o4-trackcress-source-archive . Repository https://github.com/iLanis-agent/trackcress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
