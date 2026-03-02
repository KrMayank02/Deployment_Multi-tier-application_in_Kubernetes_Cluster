# Deployment of Multi-tier (WordPress + MySQL) application in Kubernetes Cluster

**Objective:** To deploy a multi-tier MySQL application using Kubernetes with specific configurations for user roles, storage, service verification, namespace restrictions, quota limits, and data management.

**Real-time scenario:** Karen is a DevOps engineer at a tech startup. Her team has developed a new application using MySQL. Now, it is her task to deploy that application. The company plans to utilize Kubernetes for its robust container orchestration capabilities. Karen must create a Kubernetes dashboard with specific configurations, user roles, storage, service verification, and data management.

**Major Tools, Environment Used in This Project:**

- kubeadm
- kubectl
- kubelet
- Containerd
- Kubernetes Dashboard
- NFS Server

**Pre-requisites:** A Kubernetes cluster should already be set up with 3 Nodes (1 Master and 2 Worker Nodes) using kubeadm.

**High Level Project Diagram:**
----------------------------------------------------------------------------------------------------------------------------------

<img width="931" height="648" alt="image" src="https://github.com/user-attachments/assets/82f65baa-72e3-4106-ad72-702605de6156" />

----------------------------------------------------------------------------------------------------------------------------------

**High Levels Tasks/Steps:**

-	Create Kubernetes Dashboard
-	Install & Configure NFS Server, create NFS based PV & PVC
-	Create Secret for MySQL Deployment
-	Create Deployment for MySQL (attach PV, PVC)
-	Create ConfigMap and Secret for Wordpress Deployment
-	Create Deployment for Wordpress (PV not required)
-	Expose Service for WordPress and MySQL Deployment
-	Verify the Deployment of Application on web browser
-	Verify the Cluster and its workloads on Kubernetes Dashboard

# Output Result Screenshots:
-------------------------------------------------------------------------------------------------------------------------------------

MySQL Deployment, pod created in Kubernetes cluster:

<img width="917" height="263" alt="image" src="https://github.com/user-attachments/assets/f56a637f-2580-406e-ac8e-cf94a28c5055" />
-------------------------------------------------------------------------------------------------------------------------------------

Wordpress Deployment, pod created in Kubernetes cluster:

<img width="965" height="299" alt="image" src="https://github.com/user-attachments/assets/c11b0a86-1575-4af7-8984-177b29f736ff" />
------------------------------------------------------------------------------------------------------------------------------------

Verify the Deployment of 2-Tier Application by accessing the Wordpress Application on web-browser:

Access the URL: http://localhost:<wordpress-NodePort>, which is http://localhost:32658/

<img width="907" height="533" alt="image" src="https://github.com/user-attachments/assets/dbec3a19-bd01-4f06-b9c6-7cbe151ddf19" />
------------------------------------------------------------------------------------------------------------------------------------

<img width="724" height="529" alt="image" src="https://github.com/user-attachments/assets/8a0f2738-4463-4b3a-b8c3-9f217dc70784" />
------------------------------------------------------------------------------------------------------------------------------------

<img width="929" height="501" alt="image" src="https://github.com/user-attachments/assets/60287ef1-e890-4864-ab06-3fca4393edf4" />

------------------------------------------------------------------------------------------------------------------------------------

Verify the Cluster and its workloads on Kubernetes Dashboard.

Access the Kubernetes Dashboard on URL: https://localhost:31855

<img width="945" height="381" alt="image" src="https://github.com/user-attachments/assets/ae2d2255-5b4e-4da0-8673-399af3dbbb61" />
-----------------------------------------------------------------------------------------------------------------------------------

<img width="959" height="513" alt="image" src="https://github.com/user-attachments/assets/4a513b72-7b48-4ce9-8d26-04f42b8cbf8a" />

------------------------------------------------------------------------------------------------------------------------------------

**As per the requirement of the Project: The Deployment of multi-tier application (Wordpress + MySQL) in Kubernetes Cluster has been done successfully.**

**Also, Kubernetes Dashboard has been created to manage and monitor the cluster, workloads and to provide real-time insights from web base GUI.**

