# Skill-Test---2-Container-Orchestration

# Container Orchestration Skill Test

## Local Deployment

1. Installed dependencies
2. Started MongoDB
3. Started backend
4. Started both frontends

## Dockerization

Created:

- backend/Dockerfile
- frontend-basic/Dockerfile
- frontend-enhanced/Dockerfile
- docker-compose.yml

Run:

docker-compose up --build

## Kubernetes Deployment

Created:

- mongodb.yaml
- backend.yaml
- frontend-blue.yaml
- frontend-green.yaml
- frontend-service.yaml

Deploy:

kubectl apply -f k8s/

## Blue-Green Deployment Strategy

Blue:
frontend-basic

Green:
frontend-enhanced

Traffic routing controlled by Kubernetes Service selector.

Blue:

version: blue

Green:

version: green

Switch command:

kubectl edit svc frontend

Change:

version: blue

to:

version: green

This allows zero-downtime switching between application versions.

## Challenges

- Docker image visibility in Minikube
- Solved using:

eval $(minikube docker-env)

- Service selector switching for blue-green deployment


Screenshots

<img width="1889" height="515" alt="image" src="https://github.com/user-attachments/assets/93ed89c1-1192-4f27-9935-a613292691ea" />

<img width="1292" height="811" alt="image" src="https://github.com/user-attachments/assets/624e0072-b113-43cc-9f84-7f8cb0d6fe28" />

<img width="1900" height="410" alt="image" src="https://github.com/user-attachments/assets/d95f7444-97f0-42d2-a570-68f74edf5c20" />

<img width="1900" height="410" alt="image" src="https://github.com/user-attachments/assets/3711e851-f884-430a-9850-7d1911762ed2" />

<img width="1142" height="260" alt="image" src="https://github.com/user-attachments/assets/723b4866-06bb-4f92-96e3-9cb40629a5c3" />

<img width="1920" height="772" alt="image" src="https://github.com/user-attachments/assets/9066153b-7b50-4549-9bf5-6f634bb85ccf" />

<img width="1896" height="123" alt="image" src="https://github.com/user-attachments/assets/740c14bf-0f77-4ece-8a2b-f5ad598a6dbb" />

<img width="1012" height="390" alt="image" src="https://github.com/user-attachments/assets/e3ec338c-a1db-4af9-a49d-875f41eec780" />

<img width="1920" height="979" alt="image" src="https://github.com/user-attachments/assets/3d1f6e71-2c25-49bf-948a-f549f986dc8f" />

<img width="1916" height="963" alt="image" src="https://github.com/user-attachments/assets/ac36e7b9-e201-4224-baec-115cce0525d3" />

<img width="1911" height="966" alt="image" src="https://github.com/user-attachments/assets/f8495b96-ed4f-465e-83d6-63eb4fe60588" />

<img width="1569" height="427" alt="image" src="https://github.com/user-attachments/assets/fcfb76cd-872e-49ef-a4f6-d9f77fd6389a" />

<img width="1908" height="228" alt="image" src="https://github.com/user-attachments/assets/953c01ca-2cb8-467e-be1e-2a4749417405" />

<img width="1917" height="980" alt="image" src="https://github.com/user-attachments/assets/97804f73-6938-49d3-a4ea-7bf39b8bb7f4" />

<img width="1920" height="1045" alt="image" src="https://github.com/user-attachments/assets/3a1773f0-b177-41c7-8837-a9601cff3510" />

<img width="1895" height="281" alt="image" src="https://github.com/user-attachments/assets/af6ceedb-9242-429e-8c32-b024979a2d0f" />

<img width="1536" height="159" alt="image" src="https://github.com/user-attachments/assets/812df71e-6ab1-435f-985e-c05b8d598ac1" />

<img width="1887" height="1030" alt="image" src="https://github.com/user-attachments/assets/a86ef7ee-29f4-48b6-9ed3-96148f0b1283" />

<img width="1018" height="261" alt="image" src="https://github.com/user-attachments/assets/dbbc7103-46c1-4f9c-bbf2-9f0218b45de5" />

<img width="1839" height="1013" alt="image" src="https://github.com/user-attachments/assets/034c8b3f-95e3-4d3e-b019-30e946717b12" />

<img width="1878" height="1019" alt="image" src="https://github.com/user-attachments/assets/3b8834d9-a12a-4530-b9fc-cc65e31fc3c2" />

<img width="1920" height="1028" alt="image" src="https://github.com/user-attachments/assets/d1608f12-4977-4eef-a9ab-7c261015cc66" />

<img width="1904" height="169" alt="image" src="https://github.com/user-attachments/assets/da0a3cb1-7261-436a-86ee-559557c09ced" />

























