# AWS EBS Volume Resizer 🚀  

A simple **GUI-based tool** built with **Python, Tkinter, and Boto3** to automate AWS EBS volume size modifications.  

![image](https://github.com/user-attachments/assets/7501cdc9-6f75-435f-b4d6-c92cef93d773)


## 🌟 Features  
✅ **Select AWS Region** dynamically  
✅ **Fetch EBS volumes** (with names & IDs)  
✅ **Displays current volume size** before modification  
✅ **Prevents unnecessary changes** (if new size = current size)  
✅ **Confirmation alerts** before modifying EBS size  
✅ **Fully automated AWS CLI-based workflow**  

## 🛠️ **Installation**  
Step 1: Install AWS CLI
To use this tool, you need to have the AWS CLI installed and configured.

🔹 Windows:
Download the AWS CLI installer from AWS CLI Official Website
Run the installer and follow the on-screen instructions
Verify installation by running:
sh
Copy
Edit
aws --version
Expected output: aws-cli/2.x.x
🔹 macOS (via Homebrew):
sh
Copy
Edit
brew install awscli
aws --version
🔹 Linux (via package manager):
sh
Copy
Edit
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
aws --version
Step 2: Configure AWS CLI
Once AWS CLI is installed, configure it with your AWS credentials:

sh
Copy
Edit
aws configure
You'll be prompted to enter:
✅ AWS Access Key ID
✅ AWS Secret Access Key
✅ Default region name (e.g., ap-south-1 for Mumbai)
✅ Default output format (press Enter to keep default json)

Verify configuration by listing available AWS regions:

sh
Copy
Edit
aws ec2 describe-regions --output table

Step 2: Run the AWS EBS Volume Resizer Tool

⚠️ Important Notes
You must have IAM permissions to modify EBS volumes (ec2:ModifyVolume)
Ensure the new size is greater than the current size (AWS does not support shrinking EBS volumes)
Changes are irreversible, so double-check before proceeding
🚀 Now you're all set to use the AWS EBS Volume Resizer! Let me know if you need further refinements. 😊

### **2️⃣ Clone the Repository**  
```sh
git clone https://github.com/your-username/aws-ebs-resizer.git
cd aws-ebs-resizer


🤝 Contributing
Pull requests are welcome! Feel free to fork the repository and improve the tool.
