# **Trabalho realizado na Semana #3**

## **Identificação**

- O CVE-2020-0601, também conhecido como CurveBall, é uma vulnerabilidade do web browser e um spoofing attack descobertos em 2020.
- Este CVE atingiu o Microsoft CryptoAPI, uma library de programas encarregue de tratar das cryptographic functions do sistema operativo Windows 10.
- Esta vulnerabilidade afetou os motores de busca Microsoft Edge e Google Chrome.

## **Catalogação**

- Descoberto pela United States’ National Security Agency (NSA) a 14 de Janeiro de 2020, sendo corrigido pela Microsoft.
- Como tem um CVSS Score de 5.8, esta vulnerabilidade tem um nível de gravidade médio, sendo considerado pela NSA como severo.
- Esta vulnerabilidade é do tipo code execution.
- Tem uma complexidade de acesso média pois as condições de acesso são especializadas, sendo necessárias algumas pré-condições para o exploit ser bem sucedido.

## **Exploit**

- Um atacante que dê exploit a esta vulnerability pode potencialmente criar os seus próprios certificados criptográficos.
- Estes certificados simulam ser originados por um certificado legítimo, não sendo reconhecidos como malignos pelo Windows.
- O facto do atacante conseguir ultrapassar a validação dos certificados do Windows 10 permitia-lhe executar código arbitrário. 
- A principal maneira de corrigir esta vulnerabilidade foi o update de software com vista a corrigir a vulnerabilidade na Crypto API do Windows, lançado pelo mesmo.

## **Ataques**

- Salim Rashid, investigador de segurança, publicou uma prova de acesso no seu twitter pessoal.
- Nesta demonstrou ter conseguido colocar um vídeo de youtube na página inicial do github.com usando um certificado CA criado por ele.
- Oliver Lyak, investigador de segurança, publicou no seu github o código necessário para explorar esta vulnerabilidade, sendo este composto por menos de 10 linhas.


## **Fontes**
- https://www.trendmicro.com/en_us/research/20/b/an-in-depth-technical-analysis-of-curveball-cve-2020-0601.html
- https://levelup.gitconnected.com/what-is-cve-2020-0601-aka-curveball-and-why-is-it-so-dangerous-8664f8c8e9e9
- https://media.defense.gov/2020/Jan/14/2002234275/-1/-1/0/CSA-WINDOWS-10-CRYPT-LIB-20190114.PDF
- https://www.cvedetails.com/cve-details.php?t=1&cve_id=CVE-2020-0601