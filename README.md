# Building a simple Voting App using Kustomize and Kubernetes 🚀
 

## Architecture Overview 🏗️

**The Voting App consists of the following components:**

- A `Frontend Service` that serves the web application to users to **vote for their favorite pets** (cats or dogs). It is Developed using **Python Flask**.
- A `Redis Service` that **stores the votes**.
- A `Worker Service` that **processes the votes and stores them in the Postgres databas**. It is Written in **.NET**.
- A `Postgres Service` that stores the **details of the votes such as the pet name and the number of votes.**
- A `Result Service` that **displays the results of the votes**. It is Written in **Node.js**.

 

## Prerequisites 📋

Before you begin, ensure you have the following installed on your local machine:

- A **Linux Machine** with `Docker` and `Kubernetes` installed.
- With `Kustomize CLI installed` on your linux machine.

 
2. Change into the directory of the cloned repository:
```bash
cd kustomize-voting-app
```
3. Create a namespace for the Voting App using the following command:
```bash
kubectl create namespace voteapp
```
4. Deploy the Voting App on your Kubernetes cluster using the following command:
```bash
kubectl apply -k voting-app/
```
 

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contributing 🤝

Contributions are welcome! Please feel free to submit a Pull Request. If you have better ideas you can create a PR and I will merge it.

 