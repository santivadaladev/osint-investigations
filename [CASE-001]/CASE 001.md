# CASE-001 · Operazione Ghost Seller
> **Tipologia:** Network Fraud Analysis | **Settore Target:** Retail/Sportswear

## 1. Executive Summary
L'indagine è stata avviata a seguito della segnalazione di una rete di siti clone che utilizzavano asset digitali di un noto brand italiano. L'analisi ha permesso di mappare un'intera infrastruttura fraudolenta composta da 6 domini interconnessi, con server localizzati in giurisdizioni off-shore e flussi di pagamento diretti verso l'est Europa.

## 2. Analisi dell'Infrastruttura (Mapping)

### 🌐 Digital Asset Investigation
| Parametro | Risultato (Oscurato) | Note Tecniche |
| :--- | :--- | :--- |
| **URL Target** | ` - omiss - [.]com` | Sito civetta principale |
| **Hosting Provider** | [REDACTED] | Servizio con policy di scarsa cooperazione |
| **Registrar** | NameCheap, Inc. | Utilizzo di Privacy Protection (WhoisGuard) |
| **IP Address** | `185.XXX.XXX.XX` | Server condiviso con altre 23 istanze sospette |

### 🛡️ Indicatori di Compromissione (IoC)
- **Domini Correlati:** `omiss[.]net`, `omiss[.]org`
- **Mail Server:** Assenza di record SPF/DKIM (indicatori di spoofing)
- **Payment Gateway:** Reindirizzamento forzato verso `secure-checkout-gateway[.]ru`

## 3. Metodologia Investigativa

### A. Cert Transparency & Pivot Analysis
Utilizzando strumenti di monitoraggio dei log SSL (come **crt.sh**), è stato eseguito un pivot sul certificato digitale.
- **Scoperta:** Il medesimo certificato è stato emesso simultaneamente per 5 domini diversi, confermando l'ipotesi di un attacco centralizzato e non di un caso isolato.

### B. SOCMINT Analysis
Analisi dei canali social utilizzati per il traffico di referral:
- **Bot-Detection:** Identificata una rete di circa 1.200 profili automatizzati con pattern di pubblicazione sincronizzati.
- **Geolocalizzazione:** L'analisi dei metadati residui e delle tracce di login ha localizzato la gestione operativa in area Est-Europea, nonostante la sede dichiarata fosse nel Nord Italia.

### C. Forensic Image Analysis
Verifica degli asset visivi tramite **ExifTool** e **Reverse Image Search**:
- **Risultato:** Le immagini del magazzino presentate come "reali" sono state rintracciate in un database stock tedesco risalente al 2019.
- **Manipolazione:** Identificate tracce di editing digitale sui loghi tramite analisi ELA (Error Level Analysis).

## 4. Conclusioni
L'indagine si è conclusa con la produzione di un report tecnico dettagliato per il cliente, contenente:
1. Lista completa degli **IoC (Indicatori di Compromissione)**.
2. Catena di custodia delle prove digitali per fini legali.
3. Segnalazione tecnica ai registrar per l'abbattimento (Takedown) della rete.

---
[🔙 Torna al Portfolio](../../README.md)