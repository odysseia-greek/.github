# Odysseia <!-- omit in toc -->

<img alt="Mascot" height="400" src="/profile/images/mascot.png" width="400"/>

Welcome to Odysseia (Ὀδύσσεια): Embark on a Greek Language Odyssey

Just as the epic poem "Odysseia" by Homeros narrates the adventurous journey of Odysseus and his crew, the endeavor to learn Greek can feel like an odyssey in itself. Odysseia is a personal passion project that harmonizes a tapestry of my interests—ranging from the captivating world of ancient Greek history to the exhilarating challenge of devising innovative technical solutions.

As a dedicated hobbyist undertaking, this project reflects my personal journey, and any missteps in translation or interpretation of the text are entirely my own. The primary objective is to provide a platform for individuals to learn and practice ancient Greek, a language that echoes through time. While a portion of the content is presented in Dutch, the majority is delivered in English, fostering accessibility for a diverse audience. Accompanying this linguistic voyage is a comprehensive dictionary, meticulously crafted to facilitate seamless exploration.

However, please bear in mind that this project remains a work in progress, with many facets still under refinement. The aspiration is not only to foster language comprehension but also to delve into the captivating realm of ancient Greek history. Although this facet is a Work in Progress, my intention is to enrich the experience with historical context and narratives.

You can engage with this endeavor by exploring the Odysseia Greek project—dedicated to the pursuit of learning ancient Greek—accessible through https://odysseia-greek.com.

Beyond its role as a language learning tool, Odysseia Greek serves as a canvas to showcase technical expertise and experiment with a diverse array of technologies. By embarking on this journey with us, you're not only immersing yourself in the world of ancient language but also bearing witness to the fusion of passion and innovation.

Thank you for joining us on this voyage of discovery and learning. Your engagement and feedback contribute to shaping this odyssey, making it an ever-evolving endeavor that mirrors the spirit of exploration that courses through the ancient epics.
# Table of contents <!-- omit in toc -->
- [Technical docs](#technical-docs)
  - [Odyssey of Services: Navigating the Odyssey Greek Learning Platform](#odyssey-of-services-navigating-the-odyssey-greek-learning-platform)
  - [Solon Flow: Ensuring Configurations and Access](#solon-flow-ensuring-configurations-and-access)
  - [The Tracing Flow: Unveiling Insights through the Symphony of Data](#the-tracing-flow-unveiling-insights-through-the-symphony-of-data)
  - [Development Flow](#development-flow)
  - [Homecluster Setup](#homecluster-setup)
- [Attike](#attike)
  - [Aristophanes - Ἀριστοφάνης](#aristophanes---ἀριστοφάνης)
  - [Euripides - Εὐριπίδης](#euripides---εὐριπίδης)
  - [Sophokles - Σοφοκλῆς](#sophokles---σοφοκλῆς)
  - [Praxiteles - Πραξιτέλης](#praxiteles---πραξιτέλης)
- [Delphi](#delphi)
  - [Perikles - Περικλῆς](#perikles---περικλῆς)
  - [Ptolemaios - Πτολεμαῖος](#ptolemaios---πτολεμαῖος)
  - [Solon - Σόλων](#solon---σόλων)
  - [Drakon - Δράκων](#drakon---δράκων)
  - [Kleisthenes - Κλεισθένης](#kleisthenes---κλεισθένης)
  - [Peisistratos - Πεισίστρατος](#peisistratos---πεισίστρατος)
  - [Periandros - Περίανδρος](#periandros---περίανδρος)
- [Olympia](#olympia)
  - [Alexandros - Αλέξανδρος](#alexandros---αλέξανδρος)
  - [Dionysios - Διονύσιος ὁ Θρᾷξ](#dionysios---διονύσιος-ὁ-θρᾷξ)
  - [Homeros - Ὅμηρος](#homeros---Ὅμηρος)
  - [Herodotos - Ἡρόδοτος](#herodotos---ἡρόδοτος)
  - [Ploutarchos - Πλούταρχος](#ploutarchos---πλούταρχος)
  - [Sokrates - Σωκράτης](#sokrates---σωκράτης)
  - [Anaximander - Ἀναξίμανδρος](#anaximander---ἀναξίμανδρος)
  - [Anaximenes - Ἀναξιμένηςς](#anaximenes---ἀναξιμένης)
  - [Demokritos - Δημόκριτος](#demokritos---δημόκριτος)
  - [Herakleitos - Ἡράκλειτος](#herakleitos---ἡράκλειτος)
  - [Parmenides - Παρμενίδης](#parmenides---παρμενίδης)
  - [Melissos - Μέλισσος](#melissos---μέλισσος)
  - [Hippokrates - Ἱπποκράτης](#hippokrates---ἱπποκράτης)
- [Frontend](#frontend)
  - [Pheidias - Φειδίας](#pheidias---φειδίας)
- [Mykenai](#mykenai)
  - [Archimedes - Ἀρχιμήδης](#archimedes---ἀρχιμήδης)
  - [Dareios - Δαρεῖος](#dareios---δαρεῖος)
  - [Lykourgos - Λυκοῦργος](#lykourgos---λυκοῦργος)
  - [Themistokles - Θεμιστοκλῆς](#themistokles---θεμιστοκλῆς)
  - [Xerxes - Ξέρξης](#xerxes---ξέρξης)
- [Agora](#agora)
  - [Archytas - Ἀρχύτας](#archytas---Ἀρχύτας)
  - [Aristoteles - Ἀριστοτέλης](#aristoteles---Ἀριστοτέλης)
  - [Diogenes - Διογένης](#diogenes---Διογένης)
  - [Eupalinos - Εὐπαλῖνος](#Eupalinos---Εὐπαλῖνος)
  - [Plato - Πλάτων](#plato---πλάτων)
  - [Thales - Θαλῆς](#Thales---Θαλῆς)
- [Common](#common)
  - [Eratosthenes - Ἐρατοσθένης](#eratosthenes---ἐρατοσθένης)

# Technical docs

There are currently a few flows that are worth expanding upon:

## Odyssey of Services: Navigating the Odyssey Greek Learning Platform

Welcome to the Odyssey Greek Learning Platform, where ancient wisdom meets modern technology. As you embark on your journey to explore the depths of the Greek language, let us guide you through the way our services weave together to create a seamless and enriching experience.

### The Starting Point

When you access [https://odysseia-greek.com](https://odysseia-greek.com), you step onto the homepage of our application, crafted with Vue.js. From here, you can embark on your learning quest through various major modules, each named after a prominent figure in Greek history.

- **Quiz (Sokrates)**: Engage in interactive quizzes that challenge your knowledge and understanding.
- **Text (Herodotos)**: Immerse yourself in the writings of Herodotus, exploring the ancient texts.
- **Grammar (Dionysios)**: Delve into the intricate web of Greek grammar with Dionysios.
- **Dictionary (Alexandros)**: Access a treasure trove of Greek words and meanings, with more in the works.

### Seamless Navigation

As you make calls and interact with the platform, our architecture works harmoniously to provide a seamless experience. The frontend, aptly named **Pheidias**, takes your requests and forwards them to a powerful backend GraphQL proxy. This proxy connects with the necessary APIs to retrieve the information you seek. Our backend APIs are meticulously crafted using Golang, ensuring efficiency and reliability.

### The Vault of Configurations

Central to our ecosystem is **Vault**, the guardian of configurations. Every API, including our major modules and backend services, sources its configuration securely from Vault. This ensures that each component is equipped with the precise information it requires to function optimally.

### Empowering Elastic Search

Elastic Search stands as the cornerstone of our system, storing the essence of our content. The database is dynamically enriched by dedicated **Dataseeders** working tirelessly behind the scenes. Each Dataseeder exclusively populates its designated index, ensuring data integrity and organization.

### Unveiling the Unconventional

Among our Dataseeders, **Parmenides** stands out with its unique approach. This visionary Seeder places messages on a queue named **Eupalinos**. These messages are then orchestrated and processed by **Melissos**, contributing to the expansion of our dictionary.

### Initiating the Journey

To ensure a seamless start for every traveler on our platform, **Periandros** and **Drakon** work as Init Containers. They lay the foundation by creating necessary roles and provisioning user accounts for each pod.

### Guiding the Odyssey

At the helm of our platform is **Themistokles**, orchestrating and managing the Kubernetes environment. When it's time for deployment, **Archimedes**, our versatile command-line tool, steps in. Archimedes orchestrates everything from high availability setups to TLS configurations, vault management, and elastic deployments.

### Enabling TLS with Perikles

Among our heroes is **Perikles**, an ingenious service wielding an **AdmissionWebHook**. Much like the Athenian statesman, Perikles examines each service and determines if TLS is required. It then adroitly creates and updates certificates, fortifying our system's security with the same wisdom that fortified the walls of Athens.

As you navigate our platform, remember that just as the heroes of ancient Greece embarked on epic journeys, you too are on a journey of discovery and learning. Together, we explore the realms of the Greek language and culture, bridging the past and the present in a symphony of knowledge.

![Services](/profile/drawio/odysseia.drawio.png)

## Solon Flow: Managing Configurations and Access

The Solon Flow within the Odyssey Greek Learning Platform is a critical mechanism responsible for managing configurations and access across services. This process is divided into several distinct flows:

### Flow Breakdown

1. **API Flow**: Interactions between services and the Elasticsearch database are handled through this flow. APIs are permitted to fetch and manipulate data within their designated index but are strictly prohibited from deleting documents or indexes. Each API operates within its own index, ensuring separation and security.

2. **Seeder Flow**: The Elasticsearch database is enriched by Seeders through document population, though they are restricted from reading any data.

3. **Hybrid Flow**: This flow is designed to accommodate jobs or APIs that require both read and create rights. For example Melissos needs to access and write to the database. This flow is likely to disappear in future uses.

### Controlled Initiation by Periandros

**Periandros**, the Init Container, is responsible for initiating the creation of essential configurations by interfacing with Solon. Users in Elasticsearch are set up, and their credentials are securely stored in Vault. The username of each pod serves as its identity, ensuring unique access for every pod.

### Ptolemaios: The Access Gatekeeper

When a pod is launched, communication is established with **Ptolemaios**, the sidecar, which then contacts Solon to obtain a one-time Vault access token. This token is rendered invalid after use. The role and access level of the pod are evaluated by Solon based on Kubernetes annotations such as:

```yaml
spec:
  template:
    metadata:
      annotations:
        odysseia-greek/role: api
        odysseia-greek/access: dictionary
```

Once the evaluation is successful, a token is issued, enabling Ptolemaios to request the necessary configuration data from Vault.

### The Elegance of Control
A controlled balance is maintained within this system. Solon is capable of creating and deleting configurations but does not have the privilege to read them. Secure and controlled access to Vault for each pod is ensured by Ptolemaios.

Through the Solon Flow, a harmonious balance of configurations and access is achieved within the platform. Just as the ancient Greeks valued the balance of wisdom and governance, these principles are upheld in modern technology, ensuring reliability and security.

![Solon](/profile/drawio/solon-flow.drawio.png)

## The Tracing Flow: Unveiling Insights through the Symphony of Data

Within the Odyssey Greek Learning Platform, the Tracing Flow plays a pivotal role in revealing the platform's performance and interactions. This flow, composed of several interconnected components, provides a comprehensive view of system behavior and resource usage.

### Aristophanes: The Tracing Service

**Aristophanes** is the core tracing service responsible for capturing and logging traces during each API call. To ensure a detailed and accurate depiction of the platform’s state at any given moment, Aristophanes also collects metrics from **Sophokles**—a sidecar that accesses the Kubernetes Metrics Server to gather real-time data on the pod it resides in. These combined traces and metrics are then stored in Elasticsearch, with each trace identified by a unique **traceid**.

### Euripides: The GraphQL Gateway

**Euripides** serves as the GraphQL gateway that facilitates the querying of both trace and metric data. Through Euripides, users can access detailed insights into the platform’s operations, drawing from the rich data collected by Aristophanes and Sophokles.

### Aiskhylos: The Metrics Collector

**Aiskhylos** is a centrally running API that regularly gathers metrics data for pods and nodes across the system. By default, this data is collected at 180-second intervals, providing an ongoing view of resource usage and system performance.

### Praxiteles: The Frontend Interface

**Praxiteles** is the frontend interface, developed in Svelte, that connects to Euripides to present all this data to users. Praxiteles allows users to visualize traces and metrics, offering an intuitive and comprehensive view of the platform’s behavior and performance.

### Sophokles: The Pod Metrics Sidecar

**Sophokles** is a sidecar running alongside each pod, responsible for accessing the Kubernetes Metrics Server to retrieve real-time metrics such as memory and CPU usage. This data is then fed into Aristophanes to complement the traces, providing a full picture of system performance at the time of each trace.

Through the combined efforts of these components, the Tracing Flow provides a rich and detailed narrative of the Odysseia Greek Learning Platform’s operations. By capturing both traces and metrics, this flow ensures that every aspect of the platform’s performance is illuminated, offering valuable insights and fostering a deeper understanding of the system’s inner workings.


![Tracing](/profile/drawio/euripides.drawio.png)

### Example trace:

```json
{
  "__typename": "ParentTrace",
  "traceID": "eb26fd0b-3ae5-410e-94df-437505936d6e",
  "isActive": false,
  "timeEnded": "2024-08-06T07:40:30.439",
  "timeStarted": "2024-08-06T07:40:30.375",
  "totalTime": 64,
  "responseCode": 200,
  "items": [
    {
      "__typename": "StartTrace",
      "parentSpanID": "3def16ee6ddc8242",
      "spanID": "3def16ee6ddc8242",
      "method": "POST",
      "url": "/graphql",
      "host": "homeros:8080",
      "remoteAddress": "10.0.0.161:46422",
      "timestamp": "2024-08-06'T'07:40:30.375",
      "podName": "homeros-64d6dfff8b-cx9np",
      "namespace": "odysseia",
      "itemType": "trace_start",
      "operation": "answer",
      "rootQuery": "query answer{\n\tanswer(\n\t\ttheme: \"Democracy\"\n\t\tset: \"1\"\n\t\tquizType: \"media\"\n\t\tquizWord: \"Ἀθῆναι\"\n\t\tanswer: \"leader, guide\"\n\t\tcomprehensive: true\n\t) {\n\t\t\t\t... on ComprehensiveResponse {\n\t\tcorrect\n\t\tquizWord\n\t\tsimilarWords{\n\t\t\tgreek\n\tenglish\n\t\t}\n\t\tfoundInText{\n\t\t\t\t\trootword\n\t\t\t\t\tconjugations {\n\t\t\t\t\t\tword\n\t\t\t\t\t\trule\n\t\t\t\t\t}\n\t\t\t\t\tresults{\n\t\t\t\t\t\tauthor\n\t\t\t\t\t\tbook\n\t\t\t\t\t\ttext{\n\t\t\t\t\t\t\ttranslations\n\t\t\t\t\t\t\tgreek\n\t\t\t\t\t\t}\n\t\t\t\t\t}\n\t\t}\n\t}\n\t}\n}\n",
      "metrics": null
    },
    {
      "__typename": "CloseTrace",
      "parentSpanID": "3def16ee6ddc8242",
      "timestamp": "2024-08-06'T'07:40:30.439",
      "podName": "homeros-64d6dfff8b-cx9np",
      "namespace": "odysseia",
      "itemType": "trace_close",
      "responseBody": "{\"correct\":false,\"quizWord\":\"Ἀθῆναι\",\"foundInText\":{\"rootword\":\"\",\"partOfSpeech\":\"\",\"conjugations\":null,\"texts\":null},\"similarWords\":[{\"greek\":\"Ἀθηναῖος\",\"english\":\"of or relating to Athens; Athenian\"},{\"greek\":\"Ἀθήναιος\",\"english\":\"Athenaeus\"},{\"greek\":\"προδαῆναι\",\"english\":\"to know beforehand\"},{\"greek\":\"κάθημαι\",\"english\":\"sit\"}],\"progress\":{\"timesCorrect\":0,\"timesIncorrect\":0,\"averageAccuracy\":0}}",
      "metrics": null
    },
    {
      "__typename": "Span",
      "parentSpanID": "3468f5687dcaebeb",
      "spanID": "6190001aa427e1e5",
      "namespace": "odysseia",
      "timestamp": "2024-08-06'T'07:40:30.438",
      "podName": "sokrates-7664457676-ldfw5",
      "itemType": "span",
      "action": "CloseSpan",
      "status": "status code: 200",
      "took": "56.042758ms"
    },
    {
      "__typename": "Span",
      "parentSpanID": "3468f5687dcaebeb",
      "spanID": "db7e61d6b186f966",
      "namespace": "odysseia",
      "timestamp": "2024-08-06'T'07:40:30.419",
      "podName": "sokrates-7664457676-ldfw5",
      "itemType": "span",
      "action": "analyseText",
      "status": "querying Alexandros for word: αθηναι",
      "took": ""
    },
    {
      "__typename": "Trace",
      "parentSpanID": "3468f5687dcaebeb",
      "spanID": "e8a168076ddb8700",
      "method": "POST",
      "url": "/herodotos/v1/texts/_analyze",
      "host": "herodotos:5000",
      "timestamp": "2024-08-06'T'07:40:30.465",
      "podName": "herodotos-86969df479-b6847",
      "namespace": "odysseia",
      "itemType": "trace",
      "metrics": {
        "__typename": "tracingMetrics",
        "cpuHumanReadable": "11m",
        "memoryHumanReadable": "86Mi",
        "cpuRaw": 11,
        "memoryRaw": 86
      }
    },
    {
      "__typename": "Span",
      "parentSpanID": "e8a168076ddb8700",
      "spanID": "ab7faebda1b1a4ec",
      "namespace": "odysseia",
      "timestamp": "2024-08-06'T'07:40:30.467",
      "podName": "herodotos-86969df479-b6847",
      "itemType": "span",
      "action": "CloseSpan",
      "status": "status code: 200",
      "took": "7.205876ms"
    },
    {
      "__typename": "Trace",
      "parentSpanID": "3468f5687dcaebeb",
      "spanID": "abc63ae8259a725c",
      "method": "GET",
      "url": "/alexandros/v1/search?lang=greek&mode=fuzzy&searchInText=false&word=%CE%B1%CE%B8%CE%B7%CE%BD%CE%B1%CE%B9",
      "host": "alexandros:5000",
      "timestamp": "2024-08-06'T'07:40:30.400",
      "podName": "alexandros-6fdb5fc789-ttgvp",
      "namespace": "odysseia",
      "itemType": "trace",
      "metrics": {
        "__typename": "tracingMetrics",
        "cpuHumanReadable": "91m",
        "memoryHumanReadable": "102Mi",
        "cpuRaw": 91,
        "memoryRaw": 102
      }
    },
    {
      "__typename": "Trace",
      "parentSpanID": "3def16ee6ddc8242",
      "spanID": "3468f5687dcaebeb",
      "method": "POST",
      "url": "/sokrates/v1/quiz/answer",
      "host": "sokrates:5000",
      "timestamp": "2024-08-06'T'07:40:30.382",
      "podName": "sokrates-7664457676-ldfw5",
      "namespace": "odysseia",
      "itemType": "trace",
      "metrics": {
        "__typename": "tracingMetrics",
        "cpuHumanReadable": "2m",
        "memoryHumanReadable": "24Mi",
        "cpuRaw": 2,
        "memoryRaw": 24
      }
    },
    {
      "__typename": "DatabaseSpan",
      "parentSpanID": "abc63ae8259a725c",
      "spanID": "6056e24a089e58ee",
      "itemType": "database_span",
      "query": "{\"query\":{\"fuzzy\":{\"greek\":{\"fuzziness\":2,\"value\":\"αθηναι\"}}},\"size\":5}",
      "namespace": "odysseia",
      "timestamp": "2024-08-06'T'07:40:30.432",
      "podName": "alexandros-6fdb5fc789-ttgvp",
      "took": "29ms",
      "hits": 27
    },
    {
      "__typename": "DatabaseSpan",
      "parentSpanID": "3468f5687dcaebeb",
      "spanID": "fb1c3d244b7a3b0d",
      "itemType": "database_span",
      "query": "{\"query\":{\"bool\":{\"must\":[{\"match\":{\"quizType\":\"media\"}},{\"match\":{\"theme\":\"Democracy\"}},{\"match\":{\"set\":\"1\"}}]}}}",
      "namespace": "odysseia",
      "timestamp": "2024-08-06'T'07:40:30.416",
      "podName": "sokrates-7664457676-ldfw5",
      "took": "7ms",
      "hits": 1
    },
    {
      "__typename": "Span",
      "parentSpanID": "3468f5687dcaebeb",
      "spanID": "48eaa150cf2432d9",
      "namespace": "odysseia",
      "timestamp": "2024-08-06'T'07:40:30.422",
      "podName": "sokrates-7664457676-ldfw5",
      "itemType": "span",
      "action": "analyseText",
      "status": "querying Herodotos for word: αθηναι",
      "took": ""
    }
  ]
}
```

## Development flow

In order to develop locally a development flow has been setup. WIP

![Development](/profile/drawio/development-flow.drawio.png)

## Homecluster Setup

Odysseia-greek runs on a k3s platform powered by raspberry pi's. WIP

![Homecluster](/profile/drawio/homecluster.drawio.png)

# Repos and services

## Attike

https://github.com/odysseia-greek/attike

### Aristophanes - Ἀριστοφάνης

βρεκεκεκὲξ κοὰξ κοάξ.τούτῳ γὰρ οὐ νικήσετε.

Brekekekex koax koax. You never beat me in this play!

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/78/Bust_of_Aristophanes_%28cropped%29.jpg/1920px-Bust_of_Aristophanes_%28cropped%29.jpg" alt="Aristophanes" width="200"/>

Aristophanes: The witty 'tracing sidecar' of our projects, just as he penned comedies that captured the essence of Athenian society, his service follows the trails of our APIs, ensuring they reach their destinations with a dash of humor.


### Euripides - Εὐριπίδης

κακῶς φρονοῦντες· ὡς τρὶς ἂν παρ’ ἀσπίδα
στῆναι θέλοιμ’ ἂν μᾶλλον ἢ τεκεῖν ἅπαξ.

How wrong they are! I would rather stand three times with a shield in battle than give birth once.

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/67/Euripide.jpg/1024px-Euripide.jpg" alt="Euripides" width="200"/>

Euripides: Much like the dramatist's compelling narratives, this API, named after Euripides, exposes the intricate traces crafted by Aristophanes, providing a dramatic insight into the inner workings of our projects.

### Sophokles - Σοφοκλῆς

οὐ γὰρ θανεῖν ἔχθιστον, ἀλλʼ ὅταν θανεῖν
χρῄζων τις εἶτα μηδὲ τοῦτʼ ἔχῃ λαβεῖν.

For death is not the most odious thing; it is rather craving death, but lacking the means to die.

<img src="https://upload.wikimedia.org/wikipedia/commons/1/19/Sophocles_pushkin.jpg" alt="Aristophanes" width="200"/>

"Sophokles: Just as Sophocles illuminated the human condition, this service sheds light on the Kubernetes realm, bringing forth metrics that unveil the state of nodes, pods, and more, in the epic saga of system orchestration."


### Praxiteles - Πραξιτέλης

non me Praxiteles Scopasue fecit

My form Praxiteles nor Scopas hewed

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f8/Edifici_carrer_Tallers_45_Barcelona_-_03_Praxiteles.JPG/1280px-Edifici_carrer_Tallers_45_Barcelona_-_03_Praxiteles.JPG" alt="Praxiteles" width="200"/>

Praxiteles: Our Svelte SPA artistically reveals the intricate traces and metrics of our APIs, sculpting insights into a visually engaging masterpiece of performance and efficiency.

## Delphi

https://github.com/odysseia-greek/delphi

### Perikles - Περικλῆς

τόν γε σοφώτατον οὐχ ἁμαρτήσεται σύμβουλον ἀναμείνας χρόνον.

he would yet do full well to wait for that wisest of all counsellors, Time.

<img src="https://upload.wikimedia.org/wikipedia/commons/d/dd/Illus0362.jpg" alt="Perikles" width="200"/>

Perikles: A central guardian, akin to the esteemed statesman, diligently watches over our services, preserving the sacred key and certificate pairs. Just as Perikles safeguarded Athens, this role ensures the secure realm of TLS for our projects.

### Ptolemaios - Πτολεμαῖος

Ἀπεδέχετο δʼ αὐτόν, φασί, καὶ Πτολεμαῖος ὁ Ζωτήρ. καὶ ἐγκρατὴς Μεγάρων γενόμενος ἐδίδου τε ἀργύριον αὐτῷ καὶ παρεκάλει εἰς Αἴγυπτον συμπλεῖν

Ptolemy Soter, they say, made much of him, and when he had got possession of Megara, offered him a sum of money and invited him to return with him to Egypt.

<img src="https://upload.wikimedia.org/wikipedia/commons/2/21/Ptolemy_I_Soter_Louvre_Ma849.jpg" alt="Ptolemaios" width="200"/>

Ptolemaios: Much like the strategic ruler himself, this sidecar service reigns supreme by supplying the essential configurations from Vault, ensuring a secure and seamless passage for our projects through the intricate corridors of data.

### Solon - Σόλων

αὐτοὶ γὰρ οὐκ οἷοί τε ἦσαν αὐτὸ ποιῆσαι Ἀθηναῖοι: ὁρκίοισι γὰρ μεγάλοισι κατείχοντο δέκα ἔτεα χρήσεσθαι νόμοισι τοὺς ἄν σφι Σόλων θῆται - since the Athenians themselves could not do that, for they were bound by solemn oaths to abide for ten years by whatever laws Solon should make

<img src="https://upload.wikimedia.org/wikipedia/commons/1/12/Ignoto%2C_c.d._solone%2C_replica_del_90_dc_ca_da_orig._greco_del_110_ac._ca%2C_6143.JPG" alt="Solon" width="200"/>

Solon is most famous for his role as the great Athenian lawgiver following the reforms made by Drakon. His laws laid the foundation of what would become the Athenian Democracy.

### Drakon - Δράκων

ἐν τοίνυν τοῖς περὶ τούτων νόμοις ὁ Δράκων φοβερὸν κατασκευάζων καὶ δεινὸν τό τινʼ αὐτόχειρʼ ἄλλον ἄλλου γίγνεσθαι - Now Draco, in this group of laws, marked the terrible wickedness of homicide by banning the offender from the lustral water

<img src="https://www.greekboston.com/wp-content/uploads/2014/12/draco-720x484.jpg" alt="Drakon" width="200"/>

Drakon is one of the ancient lawgivers in Athens.

### Kleisthenes - Κλεισθένης

ὀστρακισμός - ostracism, introduced by Kleisthenes

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/36/Cleisthenes.jpg/532px-Cleisthenes.jpg" alt="Cleisthenes" width="200"/>

Fundamental to the forming of the Athenian democracy. The lawgiver Kleisthenes is tasked with laying the foundation upon which Perikles can later flourish.


### Peisistratos - Πεισίστρατος

καὶ Πεισίστρατος μὲν ἐτυράννευε Ἀθηνέων - So Pisistratus was sovereign of Athens

<img src="https://upload.wikimedia.org/wikipedia/commons/2/25/Ingres_-_Pisistratus_head_and_left_hand_of_Alcibiades%2C_1824-1834.jpg" alt="Pisistratus" width="200"/>

The first (known) tyrant of Athens

### Periandros - Περίανδρος

Περίανδρος δὲ ἦν Κυψέλου παῖς οὗτος ὁ τῷ Θρασυβούλῳ τὸ χρηστήριον μηνύσας· ἐτυράννευε δὲ ὁ Περίανδρος Κορίνθου - Periander, who disclosed the oracle's answer to Thrasybulus, was the son of Cypselus, and sovereign of Corinth

<img src="https://upload.wikimedia.org/wikipedia/commons/4/48/Periander_Pio-Clementino_Inv276.jpg" alt="Periandros" width="200"/>

Tyrant of Corinth.

## Olympia

https://github.com/odysseia-greek/olympia

### Alexandros - Αλέξανδρος

Ου κλέπτω την νίκην - I will not steal my victory

<img src="https://upload.wikimedia.org/wikipedia/commons/5/59/Alexander_and_Bucephalus_-_Battle_of_Issus_mosaic_-_Museo_Archeologico_Nazionale_-_Naples_BW.jpg" alt="Alexandros" width="200"/>

What could I ever say in a few lines that would do justice to one of the most influential people of all time? Alexandros's energy and search for the end of the world was relentless, so too is his search for Greek words within odysseia.

### Dionysios - Διονύσιος ὁ Θρᾷξ

Γραμματική ἐστιν ἐμπειρία τῶν παρὰ ποιηταῖς τε καὶ συγγραφεῦσιν ὡς ἐπὶ τὸ πολὺ λεγομένων - Grammar is an experimental knowledge of the usages of language as generally current among poets and prose writers

<img src="https://alchetron.com/cdn/dionysius-thrax-73e8d598-e6d3-4f5f-bb04-debff25a456-resize-750.jpeg" alt="dionysios" width="200"/>

Probably the first Greek Grammarian who wrote the "Τέχνη Γραμματική". Even though often called "the Thracian" he was most likely from Alexandria which was the hub for Greek learning for a long time.

### Herodotos - Ἡρόδοτος

Ἡροδότου Ἁλικαρνησσέος ἱστορίης ἀπόδεξις ἥδε - This is the display of the inquiry of Herodotos of Halikarnassos

<img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Marble_bust_of_Herodotos_MET_DT11742.jpg" alt="Sokrates" width="200"/>

Herodotos is often hailed as the father of history. I name he lives up to. His work (the histories) is a lively account of the histories of the Greeks and Persians and how they came into conflict. This API is responsible for passing along sentences you need to translate. They are then checked for accuracy.


### Homeros - Ὅμηρος

Αἶψα γὰρ ἐν κακότητι βροτοὶ καταγηράσκουσιν.

Hardship can age a person overnight..

<img src="https://upload.wikimedia.org/wikipedia/commons/1/1c/Homer_British_Museum.jpg" alt="Homeros" width="200"/>

Homeros: Much like the legendary poet, this GraphQL proxy weaves the threads of communication, uniting our APIs in a harmonious symphony, while enabling seamless interactions that echo the eloquent tales of the ancient epics.

### Ploutarchos - Πλούταρχος

<img src="https://upload.wikimedia.org/wikipedia/commons/0/02/Plutarch_of_Chaeronea-03-removebg-preview.png" alt="Ploutarchos" width="400"/>

Ploutarchos (or Plutarch) is most well known for his Parallel Lives, a series of books where he compares a well known Roman to a Greek counterpart.

### Sokrates - Σωκράτης

ἓν οἶδα ὅτι οὐδὲν οἶδα - I know one thing, that I know nothing

<img src="https://upload.wikimedia.org/wikipedia/commons/2/25/Raffael_069.jpg" alt="Sokrates" width="200"/>

Sokrates (on the right) is a figure of mythical propertions. He could stare at the sky for days, weather cold in nothing but a simple cloak. Truly one of the greatest philosophers and a big influence on Plato which is why we know so much about him at all. A sokratic dialogue is a game of wits were the back and forth between Sokrates and whoever was unlucky (or lucky) to be part of the dialogue would end in frustration. Sokrates was known to question anyone until he had proven they truly knew nothing. As the API responsible for creating and asking questions he was the obvious choice.

### Anaximander - Ἀναξίμανδρος

οὐ γὰρ ἐν τοῖς αὐτοῖς ἐκεῖνος ἰχθῦς καὶ ἀνθρώπους, ἀλλ' ἐν ἰχθύσιν ἐγγενέσθαι τὸ πρῶτον ἀνθρώπους ἀποφαίνεται καὶ τραφέντας, ὥσπερ οἱ γαλεοί, καὶ γενομένους ἱκανους ἑαυτοῖς βοηθεῖν ἐκβῆναι τηνικαῦτα καὶ γῆς λαβέσθαι.

He declares that at first human beings arose in the inside of fishes, and after having been reared like sharks, and become capable of protecting themselves, they were finally cast ashore and took to land

<img src="https://upload.wikimedia.org/wikipedia/commons/3/38/Anaximander.jpg" alt="Anaximander" width="200"/>

Anaximander developed a rudimentary evolutionary explanation for biodiversity in which constant universal powers affected the lives of animals.

### Anaximenes - Ἀναξιμένης

οἷον ἡ ψυχή ἡ ἡμετέρα ἀὴρ οὖσα συγκρατεῖ ἡμᾶς, καὶ ὅλον τὸν κόσμον πνεῦμα καὶ ἀὴρ περιέχει

Just as our soul, being air, constrains us, so breath and air envelops the whole kosmos.

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f0/Astrologia_%28Sterrenkunde%29_De_zeven_vrije_kunsten_%28serietitel%29%2C_RP-P-BI-6393.jpg/1920px-Astrologia_%28Sterrenkunde%29_De_zeven_vrije_kunsten_%28serietitel%29%2C_RP-P-BI-6393.jpg" alt="Anaximenes" width="200"/>

Anaximenes of Miletus: A pre-Socratic philosopher who proposed air as the fundamental substance underlying all existence.

### Demokritos - Δημόκριτος

νόμωι (γάρ φησι) γλυκὺ καὶ νόμωι πικρόν, νόμωι θερμόν, νόμωι ψυχρόν, νόμωι χροιή, ἐτεῆι δὲ ἄτομα καὶ κενόν

By convention sweet is sweet, bitter is bitter, hot is hot, cold is cold, color is color; but in truth there are only atoms and the void.

<img src="https://upload.wikimedia.org/wikipedia/commons/5/58/Rembrandt_laughing_1628.jpg" alt="Demokritos" width="200"/>

Most famous for his theory on atoms, everything can be broken down into smaller parts.

### Herakleitos - Ἡράκλειτος

πάντα ῥεῖ - everything flows

<img src="https://upload.wikimedia.org/wikipedia/commons/6/67/Raphael_School_of_Athens_Michelangelo.jpg" alt="Parmenides" width="200"/>

Herakleitos is one of the so-called pre-socratics. Philosophers that laid the foundation for the future generations. One of his most famous sayings is "No man ever steps in the same river twice".
Meaning everything constantly changes. Compare that to Parmenides. He is said to be a somber man, perhaps best reflected in the School of Athens painting where his likeness is taken from non other than Michelangelo.

### Melissos - Μέλισσος

Οὕτως οὖν ἀίδιόν ἐστι καὶ ἄπειρον καὶ ἓν καὶ ὅμοιον πᾶν.

So then it is eternal and infinite and one and all alike.

<img src="https://upload.wikimedia.org/wikipedia/commons/8/8c/Melissus_Nuremberg_Chronicle.jpg" alt="Melissos" width="200"/>

Melissus of Samos: An ancient Greek philosopher known for his contributions to Eleatic philosophy, exploring the concept of reality as a single, unchanging substance.

### Parmenides - Παρμενίδης

τό γάρ αυτο νοειν έστιν τε καί ειναι - for it is the same thinking and being

<img src="https://upload.wikimedia.org/wikipedia/commons/2/20/Sanzio_01_Parmenides.jpg" alt="Parmenides" width="200"/>

Parmenides is one of the so-called pre-socratics. Philosophers that laid the foundation for the future generations.
One of the key elements in his work is the fact that everything is one never changing thing. Therefor he is a good fit for the dataseeder. Making it like nothing every changed.

### Hippokrates - Ἱπποκράτης


ὄμνυμι Ἀπόλλωνα ἰητρὸν καὶ Ἀσκληπιὸν καὶ Ὑγείαν καὶ Πανάκειαν καὶ θεοὺς πάντας τε καὶ πάσας, ἵστορας ποιεύμενος, ἐπιτελέα ποιήσειν κατὰ δύναμιν καὶ κρίσιν ἐμὴν ὅρκον τόνδε καὶ συγγραφὴν τήνδε - I swear by Apollo Healer, by Asclepius, by Hygieia, by Panacea, and by all the gods and goddesses, making them my witnesses, that I will carry out, according to my ability and judgment, this oath and this indenture.

<img src="https://upload.wikimedia.org/wikipedia/commons/7/7c/Hippocrates.jpg" alt="Hippokrates" width="200"/>


The most well known medical professional in history. Hippokrates houses tests to see whether the other services are in good health.



## Frontend

https://github.com/odysseia-greek/pheidias

### Pheidias - Φειδίας

<img src="https://upload.wikimedia.org/wikipedia/commons/d/d7/Charles_B%C3%A9ranger_-_Replica_of_The_H%C3%A9micycle_-_Walters_3783.jpg" alt="Pheidias" width="400"/>

Pheidias (or Phidias) is one of the great artists of the Greek world, most famous for his work on the Athenian Akropolis. An apt choice for the frontend of the app.


## Mykenai


https://github.com/odysseia-greek/mykenai

### Archimedes - Ἀρχιμήδης

εὕρηκα - I found it!

<img src="https://upload.wikimedia.org/wikipedia/commons/c/c5/Archimedes_The_School_of_Athens.png" alt="Archimedes" width="200"/>

Archimedes is one of the greatest mathematicians of all time. He is also known for some nifty inventions which is why his
name has been chosen for the `ctl` tooling.

### Dareios - Δαρεῖος

<img src="https://upload.wikimedia.org/wikipedia/commons/6/67/Darius_the_great._jpg.jpg" alt="Dareios" width="200"/>

Dareios is a powerful and versatile load testing repository named after the renowned Persian Great King. This repository is specifically designed to facilitate load testing for odysseia-greek.


### Lykourgos - Λυκοῦργος

<img src="https://upload.wikimedia.org/wikipedia/commons/5/57/Lycurgus.jpg" alt="Lykourgos" width="200"/>

Lykourgos (or Lycurgus) is a semi mythical lawmaker that laid the foundation for the Spartan society with strict rules. As a deployment abides by strict rules this is a great fit.
Ansbile and Terraform scripts can be found here.

### Themistokles - Θεμιστοκλῆς

<img src="https://upload.wikimedia.org/wikipedia/commons/8/86/Illustrerad_Verldshistoria_band_I_Ill_116.png" alt="Themistokles" width="200"/>

Themistokles is argueably the greatest Greek admiral. His victory at Salamis is most well-known. As an admiral he held sway over many ships and thus over many pilots (kubernetes).
You can find all helm charts needed here.

### Xerxes - Ξέρξης

<img src="https://upload.wikimedia.org/wikipedia/commons/6/64/National_Museum_of_Iran_Darafsh_%28785%29.JPG" alt="Xerxes" width="200"/>

Xerxes was the Persian great king and invaded Greece during the second Greco-Persion war. He tested the Greeks with an army so great it was reported to drain rivers and shake the earth.


## Agora

https://github.com/odysseia-greek/agora

### Archytas - Ἀρχύτας

Ἀνάγκη γάρ ποτε τῷ ἀκριβεῖ λόγῳ τὰ πολλὰ τῶν ἀνθρώπων ὑποτεταχέναι - For many things among men are necessarily subjected to accurate reason.

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a4/Archytas_of_Taras.jpg/220px-Archytas_of_Taras.jpg" alt="Aristoteles" width="200"/>

Cache interface

### Aristoteles - Ἀριστοτέλης

Τριών δει παιδεία: φύσεως, μαθήσεως, ασκήσεως.

Education needs these three: natural endowment, study, practice.

<img src="https://upload.wikimedia.org/wikipedia/commons/a/ae/Aristotle_Altemps_Inv8575.jpg" alt="Aristoteles" width="200"/>

Aristoteles: Embodying the essence of inquiry and discovery, this interface for Elasticsearch delves into the depths of data, uncovering insights and knowledge just as the philosopher Aristotle ventured to explore the realms of knowledge and understanding.


### Eupalinos - Εὐπαλῖνος

ἀρχιτέκτων δὲ τοῦ ὀρύγματος τούτου ἐγένετο Μεγαρεὺς Εὐπαλῖνος Ναυστρόφου

The designer of this work was Eupalinus son of Naustrophus, a Megarian

<img src="https://images.squarespace-cdn.com/content/v1/57125c2c2b8dde54a34b537f/1549538816053-4XZ4KPKNX30SRC0HEGE9/a09bb315a34174f55cbe532aa2cbe715.jpg" alt="Eupalinos" width="200"/>

Eupalinos: Crafted with meticulous care, this bespoke queue embodies efficiency, orchestrating tasks with precision and grace, much like the architectural marvels created by its namesake.

### Diogenes - Διογένης

ἄνθρωπον ζητῶ

I am looking for an honest man

<img src="https://upload.wikimedia.org/wikipedia/commons/b/b1/Jean-L%C3%A9on_G%C3%A9r%C3%B4me_-_Diogenes_-_Walters_37131.jpg" alt="Diogenes" width="200"/>

"Diogenes: Emulating the spirit of seeking truth and honesty, this interface engages with Vault, unearthing secrets and guarding access, much like the philosopher Diogenes pursued genuine virtue and enlightenment."

### Plato - Πλάτων

χαλεπὰ τὰ καλά

Good things are difficult to attain

<img src="https://upload.wikimedia.org/wikipedia/commons/4/4a/Platon.png" alt="Plato" width="200"/>

Plato: The philosopher of unity and ideal forms, this package serves as a harmonizing force, encapsulating shared code that embodies the essence of perfection, fostering coherence and efficiency across our projects.


### Thales - Θαλῆς

Μέγιστον τόπος· ἄπαντα γὰρ χωρεῖ

The greatest is space, for it holds all things

<img src="https://upload.wikimedia.org/wikipedia/commons/c/c6/Illustrerad_Verldshistoria_band_I_Ill_107.jpg" alt="Thales" width="200"/>

Thales: Encompassing the vast expanse of Kubernetes operations, this interface mirrors the wisdom of Thales, bridging the gap between technology and understanding, orchestrating the intricate dance of containers with insightful precision.

## Common

### Eratosthenes - Ἐρατοσθένης

<img src="https://upload.wikimedia.org/wikipedia/commons/b/b3/Eratosthene.01.png" alt="Eratosthenes" width="200"/>

Holds fixtures in multiple repos. Eratosthenes was one of the librarians of Alexandria. He is most famous for calculating the circumference of the earth.
