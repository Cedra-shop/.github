<div align="center">
  <img src="https://avatars.githubusercontent.com/u/259970750?s=200&v=4" width="150" alt="Cedra Shop Logo" style="border-radius: 50%; border: 4px solid #d32f2f; background-color: white; margin-top: 20px; padding: 5px;">
  
  <br/><br/>
  
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.herokuapp.com?font=Outfit&weight=600&size=26&pause=1000&color=d32f2f&center=true&vCenter=true&width=600&lines=Architecture+Microservices+Distribu%C3%A9e;Go+%7C+Rust+%7C+Python+%7C+TypeScript;Intelligence+Artificielle+%26+Temps+R%C3%A9el;D%C3%A9finissons+le+futur+de+la+distribution" alt="Typing SVG" />
  </a>

  <br/><br/>

  <p align="center" style="font-size: 1.2em; color: #8b949e;">
    <b>Cedra-shop</b> redéfinit la distribution de matériel électrique grâce à une architecture technologique de pointe.<br/>
    Nous construisons une plateforme e-commerce résiliente, scalable et propulsée par l'IA.
  </p>

  <br/>

  <p align="center">
    <a href="#-architecture-système"><img src="https://img.shields.io/badge/Architecture-161b22?style=for-the-badge&logo=code-igniter&logoColor=d32f2f" alt="Architecture" /></a>
    <a href="#-stack-technique"><img src="https://img.shields.io/badge/Stack_Tech-161b22?style=for-the-badge&logo=stackshare&logoColor=d32f2f" alt="Stack" /></a>
    <a href="#-rejoignez-léquipe-dingénierie"><img src="https://img.shields.io/badge/Carrières-161b22?style=for-the-badge&logo=polywork&logoColor=d32f2f" alt="Carrières" /></a>
  </p>
</div>

<br/>

<hr style="border: 1px solid #d32f2f; opacity: 0.2;"/>

<br/>

<br/>

## Architecture Système

Notre infrastructure est conçue autour d'une architecture **Microservices orientée événements**. Nous adaptons une approche polyglotte pour tirer parti des meilleures performances de chaque technologie, du frontend jusqu'à l'orchestration des données.

<div align="center">

```mermaid
%%{init: {'theme': 'dark', 'themeVariables': { 'background': 'transparent', 'primaryColor': '#0d1117', 'primaryBorderColor': '#d32f2f', 'lineColor': '#8b949e', 'textColor': '#c9d1d9', 'fontFamily': 'Helvetica'}}}%%
flowchart LR
    subgraph Clients ["📱 Apps & Web"]
        direction TB
        App("Cedra App<br/><i>Dart</i>")
        Web("Cedra Web<br/><i>TypeScript</i>")
    end

    Gateway{{"⚡ Cedra Gateway<br/><i>Traefik</i>"}}

    subgraph Core ["🛒 E-Commerce & Core"]
        direction TB
        Temporal(["⏳ Temporal<br/><i>Go</i>"])
        Auth(["🔒 Auth<br/><i>TS</i>"])
        Commerce(["🛍️ Commerce<br/><i>Go</i>"])
        Inv(["📦 Inventory<br/><i>Go</i>"])
        Order(["🧾 Order<br/><i>Rust</i>"])
        Payment(["💳 Payment<br/><i>Go</i>"])
    end

    subgraph DataCom ["🧠 Data, Finance & Marketing"]
        direction TB
        Finance(["📊 Finance<br/><i>Rust</i>"])
        Analytics(["📈 Analytics<br/><i>Go</i>"])
        AI(["🧠 AI Engine<br/><i>Python</i>"])
        Audit(["📜 Audit<br/><i>Go</i>"])
        Marketing(["🎯 Marketing<br/><i>TS</i>"])
        Mail(["📧 Mail<br/><i>TS</i>"])
    end

    subgraph FastLayer ["⚡ Infra Layer"]
        direction TB
        Cache(["⚡ Cache<br/><i>Go</i>"])
        Realtime(["🚀 Realtime<br/><i>Go</i>"])
        B2B(["🤝 B2B<br/><i>Java</i>"])
    end

    App --> Gateway
    Web --> Gateway

    Gateway --> Core
    Gateway --> DataCom
    Gateway --> FastLayer

    Commerce -.->|Inv. Check| Inv
    Commerce -.->|Create| Order
    Order -.->|Process| Payment
    Finance -.->|Logs| Audit

    classDef nodes fill:#161b22,stroke:#d32f2f,stroke-width:2px,color:#ffffff,border-radius:6px
    classDef gateway fill:#d32f2f,stroke:#161b22,stroke-width:2px,color:#ffffff,border-radius:6px
    classDef cluster fill:transparent,stroke:#30363d,stroke-width:2px,color:#8b949e,border-radius:8px
    
    class App,Web,Auth,Commerce,Inv,Order,Payment,Finance,Analytics,AI,Audit,Marketing,Mail,Realtime,Temporal,Cache,B2B nodes;
    class Gateway gateway;
    class Clients,Core,DataCom,FastLayer cluster;
```

</div>

<br/>

<div align="center">
  <img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%">
</div>

<br/>

## 🛠 Stack Technique

Nous croyons en une approche **Polyglotte**. Chaque microservice est écrit dans le langage le plus adapté à ses contraintes de performance et de résilience.

<div align="center">
  
  <h3>📱 Frontend & Mobile</h3>
  <p>
    <img src="https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white" alt="Flutter" />
    <img src="https://img.shields.io/badge/Dart-%230175C2.svg?style=for-the-badge&logo=dart&logoColor=white" alt="Dart" />
    <img src="https://img.shields.io/badge/Next.js-black?style=for-the-badge&logo=next.js&logoColor=white" alt="Next JS" />
    <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  </p>
  <i>Applications natives iOS/Android fluides & Dashboard Web réactif.</i>
  
  <br/><br/>

  <h3>⚡ Core Backend</h3>
  <p>
    <img src="https://img.shields.io/badge/Go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white" alt="Go" />
    <img src="https://img.shields.io/badge/Rust-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white" alt="Rust" />
    <img src="https://img.shields.io/badge/Java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
    <img src="https://img.shields.io/badge/gRPC-244c5a.svg?style=for-the-badge&logo=google&logoColor=white" alt="gRPC" />
  </p>
  <i>Logique métier ultra-rapide (Go) et sécurité mémoire sans compromis pour les commandes (Rust).</i>

  <br/><br/>

  <h3>🧠 Data & IA</h3>
  <p>
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
    <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white" alt="PyTorch" />
    <img src="https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white" alt="TensorFlow" />
    <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  </p>
  <i>Modèles prédictifs et moteurs de recommandation hyper-personnalisés en temps réel.</i>

  <br/><br/>

  <h3>⚙️ Infrastructure (On-Premise)</h3>
  <p>
    <img src="https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
    <img src="https://img.shields.io/badge/HashiCorp_Nomad-151821?style=for-the-badge&logo=hashicorp&logoColor=white" alt="Nomad" />
    <img src="https://img.shields.io/badge/Valkey-%23FF4300.svg?style=for-the-badge&logo=valkey&logoColor=white" alt="Valkey" />
    <img src="https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Kafka" />
  </p>
  <i>Orchestration légère et résiliente via Nomad, Streaming d'events (Kafka) et Caching distribué ultra-rapide (Valkey).</i>

</div>

<br/>



## 🚀 Rejoignez l'équipe d'Ingénierie

**Cedra-shop** ne cherche pas de simples exécutants, nous cherchons des **ingénieurs passionnés** par la complexité, la performance brute et l'architecture distribuée à grande échelle.

<br/>

<div align="center">
  <h3>💼 Nos Défis & Postes Ouverts</h3>
  
  <br/>

  <table width="100%" style="text-align: left;">
    <tr align="center">
      <td width="50%">
        <h4>🎯 Défis Techniques</h4>
        <ul align="left">
          <li><b>Consistance Distribuée</b> : Implémentation de Saga patterns via Temporal.</li>
          <li><b>Micro-optimisations</b> : Repousser les limites de Rust pour la finance.</li>
          <li><b>MLOps Temps-Réel</b> : Scaler l'inférence de nos réseaux de neurones.</li>
          <li><b>Observabilité Massive</b> : Tracing distribué pour milliers de reqs/sec.</li>
        </ul>
      </td>
      <td width="50%">
        <h4>🔥 Postes à Pourvoir</h4>
        <ul align="left">
          <li>👨‍💻 <b>Senior Backend Engineer</b> <i>(Go / Rust)</i></li>
          <li>📱 <b>Mobile Architect</b> <i>(Flutter / Dart)</i></li>
          <li>🧠 <b>AI / Data Engineer</b> <i>(Python / PyTorch)</i></li>
          <li>⚡ <b>Site Reliability Engineer</b> <i>(Nomad / Linux)</i></li>
        </ul>
      </td>
    </tr>
  </table>
  
  <br/><br/>

  <a href="mailto:recrutement@cedra-shop.com">
    <img src="https://img.shields.io/badge/Postuler_chez_Cedra--Shop-D32F2F?style=for-the-badge&logo=minutemailer&logoColor=white" alt="Apply Now" height="45"/>
  </a>
  &nbsp;&nbsp;&nbsp;
  <a href="https://cedra-shop.com">
    <img src="https://img.shields.io/badge/Visiter_le_site_web-161b22?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website" height="45"/>
  </a>
</div>

<br/>
<br/>

<div align="center">
  <p>
    <small>
      © 2026 <b>Cedra Shop Organization</b>. All systems private & secure. <br/>
      Built with <span style="color: #d32f2f;">❤️</span> and high throughput.
    </small>
  </p>
</div>
