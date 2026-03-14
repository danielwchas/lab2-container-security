# LAB 2
## Container Security

### Skärmdumpar
Trivy Before
<p align="center">
  <img src="screenshots/trivy-before.png" alt="trivy-before.png" width="600">
</p>

Trivy After
<p align="center">
  <img src="screenshots/trivy-after.png" alt="trivy-after.png" width="600">
</p>

Gatekeeper Deny
<p align="center">
  <img src="screenshots/gatekeeper-deny.png" alt="gatekeeper-deny.png" width="600">
</p>

Gatekeeper Pass
<p align="center">
  <img src="screenshots/gatekeeper-pass.png" alt="gatekeeper-pass.png" width="600">
</p>

### Reflektion
En säker container är en mindre container. Istället för att köra en full Python kör man en slimmad version som har mycket mindre bloat. I scan-after.txt listas betydligt färre libraries än i scan-before.txt. Om ett library inte finns så behöver man inte oroa sig för att det är sårbart, eller härda just det. 
En SBOM visar vilka libraries som finns i projektet, och då är det lätt att se om man har ett library med kända sårbarheter. 
Gatekeeper ser till att man inte deployar appar med säkerhetsrisker. Det kan vara saker som att man tillåter att appen kör som root, eller fel och sårbarheter som Kubernetes inte bryr sig om. 
