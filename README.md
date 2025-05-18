# Kosovo Media Monitor API

Ez az API egy mesterséges intelligencia által vezérelt médiamonitorozó rendszer része, amely segíti a Koszovóval és Szerbiával kapcsolatos narratívák, dezinformációk és közösségi médiás trendek elemzését.

## 📌 Funkcionalitás

- Hírek keresése hírportálokról (`/news/search`)
- Közösségi média trendek lekérdezése (`/socialmedia/trending`, `/socialmedia/live`)
- Szentiment- és narratívaelemzés (`/text/analyze`)
- Botaktivitás vizsgálata (`/socialmedia/botcheck`)
- Dezinformáció-ellenőrzés (`/text/disinfo-check`)
- Narratívák időbeli követése (`/narratives/evolution`)
- Statisztikai összesítések (`/stats/summary`)
- Térbeli aktivitás (`/geo/hotspots`)
- Automatikus válaszgenerálás (`/response/generate`)
- Top influenszerek azonosítása (`/socialmedia/top-authors`)

## 🚀 Használat

1. **Futtatás előtt**: Győződj meg róla, hogy rendelkezel OpenAPI-kompatibilis eszközzel (pl. Swagger UI, Postman).
2. **API dokumentáció betöltése**:
   - Nyisd meg [https://editor.swagger.io](https://editor.swagger.io)
   - Másold be a `api-spec/openapi.yaml` fájl tartalmát

## 🔐 Hitelesítés

Az API `X-API-Key` fejlécen keresztül használható. Példa:
```http
GET /news/search HTTP/1.1
Host: api.kosovo-media-monitor.ai
X-API-Key: YOUR_API_KEY
