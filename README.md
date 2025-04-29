# free-Lightning.ai-runners
CI/CD GPU Runners for ML Projects

## How to Run This Repo

1. **Sign Up for Lightning.ai**  
   Sign up at [Lightning.ai](https://lightning.ai/sign-up) and get your **API Key** and **User ID** from [here](https://lightning.ai/<username>/<teamspace>/studios?settings=keys).

2. **Set Up GitHub Actions**  
   Copy the GitHub Actions workflow from the `/.github/workflows` folder into your own project. Make sure to set up the **API Key** and **User ID** as secrets in your GitHub repository settings.

3. **Trigger the Workflow**  
   The workflow is set up to run on **workflow_dispatch**, which means you can trigger it manually from the GitHub UI.

---

## Article Location

You can read the full article explaining this process on Medium:  
[Use Free Lightning.ai CI/CD GPU Runners for Your ML Project – MLOps Series 1/3](https://medium.com/p/e69617d6b954)

---

## GitHub Actions Workflow

The provided GitHub Actions workflow automates the following:

- Installs necessary dependencies (including the Lightning SDK).
- Creates a Lightning.ai Studio with a free T4 GPU.
- Clones your GitHub repository and installs the dependencies.
- Runs your model training script remotely on the GPU.
- Stops and deletes the studio after training is complete.

This workflow enables **CI/CD model training** using free GPU resources, helping to save costs while speeding up the training process.

---

## Contributions

Contributions are welcome! If you would like to improve this project, feel free to open a pull request or report any issues. Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.

---

## About the Author

This repository and the accompanying article were created by **Jakub**. Jakub is a DevOps engineer and a machine learning enthusiast with experience in building CI/CD pipelines and working with cloud infrastructure. He is a member of the **GHOST** (Group Of Horribly Optimistic STatisticians) team, and is passionate about leveraging cutting-edge technologies to optimize machine learning workflows.

---

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
