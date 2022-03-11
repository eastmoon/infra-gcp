# [Google Cloud Platform](https://cloud.google.com/?hl=zh-tw)

GCP 是一項使用了 Google 核心基礎架構、資料分析和機器學習技術的雲計算服務。其主要提供軟體開發商基礎設施託管和開發人員產品技術支援，用於構建從簡單網站到複雜應用程式的一系列程式，並提供一系列模塊化的基於雲的服務和大量開發工具。

對於 GCP 操作有兩個主要方式，一是採用 GCP 提供的網頁操作平台、二是採用 SDK 透過 CLI (Command line) 進行遠端操作。

+ [Google Cloud Platform console](https://console.cloud.google.com/)
+ [Google Cloud SDK](https://cloud.google.com/sdk/gcloud/?hl=zh-tw)
  - [SDK 初始化](https://cloud.google.com/sdk/docs/authorizing)
  - [SDK 授權](https://cloud.google.com/sdk/docs/authorizing)

需注意，Google Cloud Platform SDK 是一套用於對 GCP 溝通的開發工具，因此，必需經過初始化才可正確的存取對應帳號的 GCP ；但 SDK 可同時存取多個帳戶，方法可參閱上述連結。

## 操作

+ [建立與管理](./docs/create)
+ [gcloud 初始化](./docs/initial)
+ [gcloud 操作](./docs/operation)

## 文獻

### Googld Cloud Platform

+ [三分鐘在 GCE 上部署 Docker Container](https://www.mile.cloud/zh-hant/deploying-container-on-google-compute-engine/)
> 若要在 Compute Engine VM 或代管執行個體群組上部署及啟動容器，請提供 Docker 映像檔名稱，並設定在 VM 或執行個體範本建立容器時，該容器應以何種方式執行。
>
> Compute Engine 會負責處理其餘的工作，包括提供已安裝 Docker 的最新 Container-Optimized OS 映像檔，並在啟動 VM 時啟動容器。

+ [在 Google Cloud Platform 上使用 GPU 和安裝深度學習相關套件](https://medium.com/@kstseng/%E5%9C%A8-google-cloud-platform-%E4%B8%8A%E4%BD%BF%E7%94%A8-gpu-%E5%92%8C%E5%AE%89%E8%A3%9D%E6%B7%B1%E5%BA%A6%E5%AD%B8%E7%BF%92%E7%9B%B8%E9%97%9C%E5%A5%97%E4%BB%B6-1b118e291015)

### [Kubernetes](https://cloud.google.com/container-engine/?hl=zh-tw)

依據 [GKE 系列文章(一) – 為什麼使用 Kubernetes](https://blog.gcp.expert/kubernetes-gke-introduction/)，Google 於2015年釋出Kubernetes(簡稱K8S)，其主要功能是實踐 Docker 容器依據流量、用量做到動態部屬的管理設計機制。

『當開發維運時，最希望的就是在部署後持續監控，當任一台伺服器流量過頭的時候，希望可以自動擴展；當流量很低迷時，可以自動縮減伺服器。除此之外，最重要的是，當一台伺服器掛點後，希望可以自動修復，而且隨時必須保持服務實例的個數。以上很多功能Docker都可以幫您做到，並利用容器來提供服務。這樣的服務型態被稱作CaaS(Container as a Service)，看起來一切都很美好。但是Docker容器不是萬能，在容器/服務個數越來越複雜的情況下，如何管理叢集和服務的生命週期，將會是各家容器編排管理(orchestration)的能力。』

+ [在 GCP 中建立 k8s 叢集](https://ithelp.ithome.com.tw/articles/10193961)
+ [Kubernetes 佈署 Docker Image](https://blog.johnwu.cc/article/gcp-kubernetes-deploy-docker-image.html)
