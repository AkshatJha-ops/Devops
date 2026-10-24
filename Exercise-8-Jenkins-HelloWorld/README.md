# Assignment 8: Creating a Hello World Jenkins Job

## 1. Aim
To create and execute a Freestyle project in Jenkins that prints a Hello World message and verify the build output.

## 2. Prerequisites
- Jenkins installed and running
- Java Development Kit (JDK) configured
- Access to the Jenkins dashboard through a web browser

## 3. Procedure

### Step 1: Open Jenkins
Open `http://localhost:8080` in a web browser and log in to the Jenkins dashboard.

### Step 2: Create a Freestyle Project
1. Click **New Item**.
2. Enter the job name `HelloWorld`.
3. Select **Freestyle project**.
4. Click **OK**.

### Step 3: Configure the Build
1. Open the job configuration page.
2. Navigate to the **Build Steps** section.
3. Select **Execute Windows batch command**.
4. Enter the following command:

```bat
echo Hello, Jenkins!
```

5. Click **Save**.

### Step 4: Execute the Job
1. Open the `HelloWorld` job.
2. Click **Build Now**.
3. Select the latest build and open **Console Output**.

## 4. Expected Output

```text
Hello, Jenkins!
Finished: SUCCESS
```

## 5. Result
A Freestyle project named `HelloWorld` was created and executed successfully in Jenkins. The expected message was displayed in the console output.

## 6. Learning Outcome
- Learned how to create a Freestyle project in Jenkins.
- Learned how to configure a Windows batch build step.
- Learned how to execute a Jenkins build and inspect its console output.
