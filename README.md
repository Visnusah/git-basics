# git-basics

```markdown
# Software Design Repository

This repository is a step-by-step guide to setting up a new Git repository, creating and modifying files, committing changes, creating and merging branches, and pushing the changes to a remote repository on GitHub.

## Prerequisites

Before you begin, you'll need to have the following installed on your system:

- Git (https://git-scm.com/downloads)
- A text editor or an IDE of your choice
- A GitHub account (https://github.com)

## Getting Started
### 1. Configure Git User Name and Email (if needed)

Before running the `git push` command, you may need to configure your Git user name and email address using the following commands:

```
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

Replace `"Your Name"` and `"your@email.com"` with your actual name and email address.
### 2. Create a New Repository

#### macOS

```zsh
# Create a new directory for the project
mkdir software_design
cd software_design

# Initialize a new Git repository
git init

# Create a new remote repository on GitHub
# (Open your web browser, navigate to GitHub, and create a new repository named "software_design")
# Copy the URL of the new repository (e.g., https://github.com/your_username/software_design.git)

# Connect the local repository to the remote repository
git remote add origin https://github.com/your_username/software_design.git
```

#### Windows

```
# Create a new directory for the project
mkdir software_design
cd software_design

# Initialize a new Git repository
git init

# Create a new remote repository on GitHub
# (Open your web browser, navigate to GitHub, and create a new repository named "software_design")
# Copy the URL of the new repository (e.g., https://github.com/your_username/software_design.git)

# Connect the local repository to the remote repository
git remote add origin https://github.com/your_username/software_design.git
```

### 3. Create and Upload File

#### macOS

```zsh
# Create a file named index.txt in your local repository
printf "Hello, GitHub!" > index.txt

# Add the file to the staging area
git add index.txt

# Commit the file with the message "First Commit"
git commit -m "First Commit"

# Push the changes to the remote repository
git push -u origin master
```

#### Windows

```
# Create a file named index.txt in your local repository
echo Hello, GitHub! > index.txt

# Add the file to the staging area
git add index.txt

# Commit the file with the message "First Commit"
git commit -m "First Commit"

# Push the changes to the remote repository
git push -u origin master
```

### 4. Make Changes and Commits

Follow the same pattern for both macOS and Windows:

```
# Change 1
echo "Test written 1" >> index.txt  # For macOS, use: printf "Test written 1\n" >> index.txt
git add index.txt
git commit -m "Second Commit"
git push

# Change 2
echo "Test written 2" >> index.txt  # For macOS, use: printf "Test written 2\n" >> index.txt
git add index.txt
git commit -m "Third Commit"
git push

# Change 3
echo "Test written 3" >> index.txt  # For macOS, use: printf "Test written 3\n" >> index.txt
git add index.txt
git commit -m "Fourth Commit"
git push

# Change 4
echo "Test written 4" >> index.txt  # For macOS, use: printf "Test written 4\n" >> index.txt
git add index.txt
git commit -m "Fifth Commit"
git push

# Change 5
echo "Test written 5" >> index.txt  # For macOS, use: printf "Test written 5\n" >> index.txt
git add index.txt
git commit -m "Sixth Commit"
git push
```

### 5. Create and Merge Branch

Follow the same pattern for both macOS and Windows:

```
# Create a new branch named 'Branch_1' from the main/master branch
git branch Branch_1

# Switch to the 'Branch_1' branch
git checkout Branch_1

# Modify index.txt in this branch
echo "New branch test written 1" >> index.txt  # For macOS, use: printf "New branch test written 1\n" >> index.txt
git add index.txt
git commit -m "Branch First Commit"
git push origin Branch_1
```

### 6. Merge Branch and Push Changes

Follow the same pattern for both macOS and Windows:

```
# Switch back to the main/master branch
git checkout master

# Merge the changes from 'Branch_1' into the main/master branch
git merge Branch_1

# Push the merged changes to the remote repository
git push
```



That's it! You've successfully set up a new Git repository, created and modified files, committed changes, created and merged branches, and pushed the changes to a remote repository on GitHub.

## Contributions

Contributions to this repository are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE)
You can copy and paste this content into a new file named `README.md` in your repository, and it will be displayed beautifully on GitHub. Additionally, you can customize the content according to your specific needs or project requirements.
