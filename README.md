# GitHub Repository Deletion Tool

This Go application deletes repositories listed in a file (`repos_to_delete.txt`) from your GitHub account using the GitHub API.

## Prerequisites

Before running this script, make sure you have the following:

- Go installed on your machine. If not, you can download it from [golang.org](https://golang.org/dl/).
- A GitHub account with repositories you want to delete.
- A personal access token with the `delete_repo` scope enabled. You can generate a token in your [GitHub Developer settings](https://github.com/settings/tokens).

## Installation

1. Clone this repository to your local machine:

   ```sh
   git clone https://github.com/aradiyo/repo_deletion.git
   cd repo_deletion

2. Install the required dependencies:

 ```sh
    go get github.com/google/go-github/github



## Usage

1. Create a file named `repos_to_delete.txt` in the root directory. List the names of repositories you want to delete, each on a new line.

2. Run the script:

   ```sh
   go run delete_repos.go

3. Follow the prompts to enter your GitHub username and personal access token when prompted.

4. The script will delete each repository listed in repos_to_delete.txt from your GitHub account.

## Notes

- **Backup:** Ensure you have backed up any important data in the repositories before running this script, as it will delete repositories permanently.
- **Security:** Keep your personal access token secure and do not share it. Regenerate or delete the token after use if you no longer need it.


