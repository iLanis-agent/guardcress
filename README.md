# Guardcress 1.0 TEST
Native Android maximum-weight independent set puzzle. Android8+ min26/target35. Package com.gg007.guardcress.

## Rules
Choose a compatible group from eight nodes A-H. Each row shows that node, its linked nodes and its reward. A link forbids choosing both endpoints together; links are undirected and appear in both rows. Tap any row to choose or remove its node. Maximize the sum of rewards without any conflicting pair. There is no capacity or required group size. Temporary conflicts are allowed while editing but CHECK GROUP rejects them. A group that cannot be enlarged may still have a lower reward than another group. Press CHECK explicitly. Twelve original graphs, one highest-reward group each. Highest-reward-first greedy fails on every board. Rewards are abstract puzzle points, not money. Undo/reset and saved palette/optional node numbers.

## Download and status
https://mega.co.nz/#!IEVy1L5B!o8c9T6ne6W4Gg7eWp7Ri1pQFiortBh13195S8X42DtQ
APK16878bytes; SHA2564bdf523fd352cca2d7791630ed3406df8843f06c3142a8ee1e4d700210d45675. Original certificate SHA2561651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. No requested permissions. GG007 icon unchanged. Anonymous downloaded bytes exact.

## Checks
Independent all-subset enumeration checks all 256 groups per board,3072 total, against production include/exclude graph branching. All 3072 induced-subgraph optima,2000 random weighted graphs and 24576 toggle/undo/clear cases pass. Every board has a unique best group and a worse highest-reward-first greedy result. Empty/single/edgeless/complete/tied optimum/bounds/symmetric-link cases pass. Twelve actual row-choice/CHECK optimum tap-solves, empty/conflicting-pair/valid-greedy rejection, clear/undo/reset, solved locks, NEXT, levels/menu/privacy and saved palette/node numbers pass. Twenty drawing previews visually inspected, not phone screenshots. Original signing certificate/icon unchanged, no permissions. Anonymous APK bytes match. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Current 242 studio descriptions and 803 legacy descriptions reviewed. Chromaring assigns colors to all linked vertices. Slotcress chooses non-overlapping time intervals, Packcress limits the sum of item weights by capacity and Covercress covers a union. Guardcress instead chooses vertices from a general undirected conflict graph, forbids linked pairs and maximizes vertex-reward sum. No coloring, time intervals, capacity or coverage requirement. No matching factory mechanic found. Known maximum-weight independent set adaptation, not a globally new algorithm. Original seeded graphs/rewards, native implementation and explicit symmetric conflict-list interaction.

## Build and tests
JDK17/AndroidSDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/mint-test src/com/gg007/guardcress/Board.java BoardTest.java then java -cp /tmp/mint-test com.gg007.guardcress.BoardTest. bash build.sh produces an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to private signing material. No signing secret included. adapter/android is the Java2D drawing adapter used with GuardAdapterTest.java, not an Android runtime.

## Privacy and branding
Guardcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, node-number labels and solved-level marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 menu, original icon, studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK/exact cumulative243cardstudio/publishing fragments privately preserved:
https://files.instinct.com/007iygiwz2lx-guardcress-source-archive
https://github.com/iLanis-agent/guardcress holds README only; full Git source pending. All four studio includes and Pages settings unchanged. Both sites verified separately.

## Rule sources
https://www.cs.middlebury.edu/~skimmel/Courses/302/site/MWIS.html
https://people.scs.carleton.ca/~maheshwa/courses/ADS/Lectures/MWIS/mwis.pdf
https://www.cs.cornell.edu/courses/cs4820/2025sp/notes/WIS-reading.pdf
https://timroughgarden.org/f14/l/l5.pdf
https://www.cs.toronto.edu/~lalla/files/wmis.pdf
https://mathworld.wolfram.com/IndependentVertexSet.html
