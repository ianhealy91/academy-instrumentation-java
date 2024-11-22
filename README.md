
# Honeycomb Academy: Sample Meminator App Answer Key

***This is a demo app, don't run it in production!***

This branch is an answer key. All code modifications and additions are commented out, along with short directions. Please refer to the lab activities in Honeycomb Academy for the comprehensive direction set.

Below are instructions for running the application. This contains a sample application for use in Honeycomb Academy lab activities. This app has 4 services. It generates images by combining a randomly chosen picture with a randomly chosen phrase.

## Introduction

Hello! Welcome to the **Instrumentation for OpenTelemetry Java** course lab.

1. Take a look at this app. 
2. Before you can do make any changes, you need to run this app.
3. Then, connect this app to Honeycomb.
4. See what the traces look like.
5. Improve the traces.


## Running the application

To run this app, you can use GitPod or Codespaces.

Once you run the application, you can send traces to Honeycomb. Then you can practice improving the instrumentation for better observability.

### GitHub Codespaces setup

Open the repository on GitHub. Open the `<> Code` dropdown down menu.

Select the `Codespaces` tab. Create a codespace on main.

### GitPod setup

Go to [Gitpod](https://gitpod.io/#https://github.com/honeycombio/academy-instrumentation-java) to open the repository.

Confirm the workspace creation. You can work in the browser with VS Code Browser or in your local code editor. The default settings are acceptable. 

Once you are in the code editor, run `docker compose up` in the code editor's terminal. To stop running the application, run `ctrl+c`. Then run `docker compose down` to remove the container.

### Local development setup

You also have the option to run this application locally.

First, clone this repository.

```bash
git clone https://github.com/honeycombio/academy-instrumentation-java.git
```

Install Docker: https://docs.docker.com/get-docker/


### Run the app

`./run`

(This will run `docker compose` in daemon mode, and build containers.)

Access the app:

[http://localhost:10114]()

After making changes to a service, you can tell it to rebuild just that one:

`./run [ meminator | backend-for-frontend | image-picker | phrase-picker ]`

### Try it out

Visit [http://localhost:10114]()

> If you are using **GitPod**, the address may not be localhost. When running, the VSC environment will ask you if you want to expose the ports to public. Select Yes, and you will see the external address and port 10114, to which you can then click the globe icon to show it on a new tab.

Click the "GO" button. Then wait.

> **NOTE** ⚠️ If you run the application for the first time, the result image may not load up properly. In that case, reload the page, and try again a few times.

### Stop the app

`./stop`
