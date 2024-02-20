# Parancslista

## Javascript
- `console.log('message')` - kiírja a konzolra a message-t
- `alert('message')` - kiírja egy alertablakba a message-t
- `.map()` - végigiterál egy tömbön
- `.filter()` - szűri a tömböt
- `.reduce()` - összegzi a tömb elemeit
- `.sort()` - sorba rendezi a tömböt
- `.forEach()` - végigiterál egy tömbön
- `.find()` - megkeresi a tömbben az első elemet
- `.split()` - szétválasztja a stringet, atributumként megadott karakter alapján. Default: minden karaktert szétválaszt
### Javascript helper
 - `random szám` 
   - `function rand(min, max) {
     return Math.floor(Math.random() * (max - min +1))+min;
     }`
   - `rand(1, 10);` - 1 és 10 közötti random szám
      


### Matematikai fogalmak
- `Math.PI` - pi értéke
- `Math.round()` - kerekít
- `Math.floor()` - lefelé kerekít
- `Math.ceil()` - felfelé kerekít
- `szám%2` - páros vagy páratlan
- `számtai Sorozat`- Számok köszti összeg egyenlő.


## TypeScript
- `npm install -g typescript` - telepíti a TypeScriptet
- `tsc --init` - inicializálja a TypeScript konfigurációs fájlt
- `tsc` - lefordítja a TypeScript fájlokat
- `tsc -w` - figyeli a fájlokat és ha változik, lefordítja

## Git
- `git init` - inicializálja a gitet
- `git add .` - hozzáadja a fájlokat a stagehez
- `git commit -m "message"` - commitolja a fájlokat
- `git push` - feltölti a fájlokat a távoli repóba
- `git pull` - letölti a fájlokat a távoli repóból
- `git clone url` - klónozza a távoli repót
- `git status` - megmutatja a változásokat
- `git log` - megmutatja a commitokat
- `git branch` - megmutatja a brancheket
- `git checkout -b branch` - létrehoz egy branchet
- `git checkout branch` - átvált egy branchre
- `git merge branch` - összefűzi a branchet a jelenlegivel
- `git branch -d branch` - törli a branchet
- `git push origin --delete branch` - törli a távoli branchet

## Angular
- `npm install -g @angular/cli` - tele
- `ng new my-app` - létrehozza az alkalmazást my-app helyén a nevet  határozod meg. (Route kell, SCSS vagy CSS választható)
- `cd my-app` - belép a mappába
- `ng serve` - elindítja a fejlesztői szervert
- `ng generate component my-component` - létrehoz egy komponenst
- `ng generate service my-service` - létrehoz egy szolgáltatást
- `ng add @ng-bootstrap/ng-bootstrap` - hozzáadja a Bootstrapet
- `npm install bootstrap` - telepíti a Bootstrapet app css-be kell importálni
`@import '~bootstrap/dist/css/bootstrap.min.css';`

### Angular helper
- `<tag [ngClass]>` - classokat adhatunk meg változóként
- `<tag [ngStyle]>` - stílusokat adhatunk meg változóként
- 
- `<tag *ngFor="let item of items">` - végigiterál egy tömbön
- `<tag *ngSwitch="condition">` - feltételhez kötött megjelenítés'
- `<tag *ngIf="condition">` - feltételhez kötött megjelenítés
- `<tag [(ngModel)]="var">` - kétirányú adatkötés
- `<tag (event)="function()">` - eseményre futtatott függvény
- `<tag (click)="function()">` - kattintás eseményre futtatott függvény
### Angular routing
-  Az app-routing.module.ts-ben kell definiálni a routeokat. A routes constans ba `[{path: 'path', component: Component}]` formában. a path: '' az alapértelmezett útvonal. (Url: localhost:4200/path). A component: Component a komponens neve, amit megjelenít.


## Node server
- `node server.js` - elindítja a szervert
- `node teszt.js` - futtatja a teszt.js fájlt
- A server futatásához kell a http modul. `const http = require('http');`
- A server futtatásához kell egy port. `const port = 3000;`
- A server futtatásához kell egy request és egy response. `http.createServer((req, res) => {res.end('Hello World!');}).listen(port);`
- A kérésbe befűzhető egy statuscode. 
  - `res.writeHead(200, {'Content-Type': 'text/html'});` 
  - `res.setHeader('Content-Type', 'text/html');` + `res.statusCode = 200;`
- A `server.listen(port, () => {console.log('Server is running...');});` fügvényel inditható el a szerver.
- A szerver össze álitható a hozzá készűlt tesztből.



## MongoDB
- `mongod` - elindítja a mongodbat
- `mongo` - elindítja a mongo shellt
- `show dbs` - megmutatja az adatbázisokat
- `use db` - használja az adatbázist
- `db.collection.find()` - lekérdezés
- `db.collection.insert()` - beszúrás
- `db.collection.update()` - frissítés
- `db.collection.remove()` - törlés
- `db.collection.drop()` - törlés
- `db.collection.createIndex()` - index létrehozása
- `db.collection.getIndexes()` - indexek lekérdezése
- `db.collection.dropIndex()` - index törlése
- `db.collection.aggregate()` - aggregáció
- `db.collection.distinct()` - egyedi értékek lekérdezése
- `db.collection.count()` - rekordok számának lekérdezése
- `db.collection.mapReduce()` - map-reduce
- `db.collection.bulkWrite()` - tömeges írás
- `db.collection.getShardDistribution()` - shard eloszlás lekérdezése
- `db.collection.getShardVersion()` - shard verzió lekérdezése
- `db.collection.getShardMap()` - shard térkép lekérdezése
- `db.collection.getShardTagRange()` - shard tag tartomány lekérdezése