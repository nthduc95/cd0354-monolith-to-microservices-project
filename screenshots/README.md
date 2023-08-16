# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed
  <img width="1512" alt="Screenshot 2023-08-16 at 21 39 53" src="https://github.com/nthduc95/cd0354-monolith-to-microservices-project/assets/119287881/c2a483b1-ce62-44d8-b2e5-e6651418a375">
<img width="1512" alt="Screenshot 2023-08-16 at 21 40 13" src="https://github.com/nthduc95/cd0354-monolith-to-microservices-project/assets/119287881/43a38705-9f8a-42d0-b274-1e8a0ba1114b">
<img width="1512" alt="Screenshot 2023-08-16 at 21 40 19" src="https://github.com/nthduc95/cd0354-monolith-to-microservices-project/assets/119287881/4bb3ed4e-3e49-448c-b0d9-3ea1c42c26a1">
<img width="1512" alt="Screenshot 2023-08-16 at 21 40 25" src="https://github.com/nthduc95/cd0354-monolith-to-microservices-project/assets/119287881/08f2d87a-a3a8-4c79-8114-4c4491fd80ce">
<img width="1512" alt="Screenshot 2023-08-16 at 21 40 30" src="https://github.com/nthduc95/cd0354-monolith-to-microservices-project/assets/119287881/f8f3c3d7-73f4-4556-9434-0696f18e5980">

* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)
  => Because I had problems with my travis's account, I used Github action instead of travis.
  https://github.com/nthduc95/cd0354-monolith-to-microservices-project/blob/main/.github/workflows/build.yml
  
* Travis CI showing a successful build and deploy job
  Here is my CI Git action uccessful build and deploy job:
  https://github.com/nthduc95/cd0354-monolith-to-microservices-project/actions
  
## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
<img width="1512" alt="Screenshot 2023-08-16 at 21 31 44" src="https://github.com/nthduc95/cd0354-monolith-to-microservices-project/assets/119287881/a6ff49d8-6897-44e5-8e68-dd8a09a04226">

* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
<img width="1512" alt="Screenshot 2023-08-16 at 21 33 08" src="https://github.com/nthduc95/cd0354-monolith-to-microservices-project/assets/119287881/9a81f4a1-bce4-4cd8-b4b9-d793190bc023">
<img width="1512" alt="Screenshot 2023-08-16 at 21 33 21" src="https://github.com/nthduc95/cd0354-monolith-to-microservices-project/assets/119287881/7a1218be-9e90-4c2d-b3f8-9021ff374509">
<img width="1512" alt="Screenshot 2023-08-16 at 21 33 27" src="https://github.com/nthduc95/cd0354-monolith-to-microservices-project/assets/119287881/5d58397b-6b42-4de7-af36-2c953cfaf33d">

* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
<img width="1512" alt="Screenshot 2023-08-16 at 21 33 53" src="https://github.com/nthduc95/cd0354-monolith-to-microservices-project/assets/119287881/8b52708c-b640-4b87-973a-8e70f5e23760">

* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
<img width="1512" alt="Screenshot 2023-08-16 at 21 34 42" src="https://github.com/nthduc95/cd0354-monolith-to-microservices-project/assets/119287881/d93de089-822d-4e3b-822e-5e8e84565fb9">
