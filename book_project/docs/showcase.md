# GenAI Project Showcase

This page showcases a collection of projects and code snippets that demonstrate the use of Generative AI in various software development tasks.

## 1. GitHub Repository Scraper

**Description:** A tool to scrape GitHub repositories for file contents and metadata. It uses the GitHub API to recursively fetch directory contents and file data.

**Code (Python):**
```python
import os
import base64
from github import Github
from github import GithubException

def get_file_contents_from_github_repo(repo_name, folder_path="", branch="main"):
    g = Github(os.getenv("GITHUB_TOKEN"))
    try:
        repo = g.get_repo(repo_name)
        contents = repo.get_contents(folder_path, ref=branch)
        file_contents = {}

        if not isinstance(contents, list):
            contents = [contents]

        for content_file in contents:
            if content_file.type == "dir":
                file_contents.update(get_file_contents_from_github_repo(repo_name, content_file.path, branch))
            else:
                try:
                    file_content = base64.b64decode(content_file.content).decode("utf-8")
                    file_contents[content_file.path] = file_content
                except (UnicodeDecodeError, GithubException) as e:
                    print(f"Error decoding or accessing file {content_file.path}: {e}")
        return file_contents
    except GithubException as e:
        print(f"Error accessing repository or folder {repo_name}/{folder_path}: {e}")
        return {}

def scrape_github_repo(repo_name, branch="main"):
    return get_file_contents_from_github_repo(repo_name, branch=branch)

# Example usage:
# repo_name = "your_username/your_repo"
# all_files = scrape_github_repo(repo_name)
# for file_path, content in all_files.items():
#     print(f"File: {file_path}\nContent:\n{content}\n")
```

**[View on GitHub](https://github.com/your-username/your-repo/path/to/scraper)**

---

## 2. Web Automation with Selenium

**Description:** A web automation script using Selenium to perform a Google search and extract the results.

**Code (Python):**
```python
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.keys import Keys
from selenium.webdriver.chrome.service import Service
from webdriver_manager.chrome import ChromeDriverManager

def perform_google_search(query):
    driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()))
    driver.get("https://www.google.com")
    search_box = driver.find_element(By.NAME, "q")
    search_box.send_keys(query)
    search_box.send_keys(Keys.RETURN)
    # You can add more code here to process the search results
    driver.quit()

# Example usage:
# perform_google_search("Generative AI in Software Development")
```

**[View on GitHub](https://github.com/your-username/your-repo/path/to/selenium-script)**

---

## 3. GitHub PR Commenting Bot

**Description:** A bot that comments on GitHub pull requests. It uses the GitHub API to post comments.

**Code (TypeScript):**
```typescript
import { Octokit } from "@octokit/rest";

async function commentOnPR(owner: string, repo: string, prNumber: number, comment: string) {
  const octokit = new Octokit({ auth: process.env.GITHUB_TOKEN });
  await octokit.issues.createComment({
    owner,
    repo,
    issue_number: prNumber,
    body: comment,
  });
}

// Example usage:
// commentOnPR("your-username", "your-repo", 123, "This is a comment from my bot!");
```

**[View on GitHub](https://github.com/your-username/your-repo/path/to/pr-bot)**

---

## 4. React UI Components

**Description:** A set of React UI components built with TypeScript, including a `Text` component and a `VStack` for vertical layout.

**Code (TSX):**
```tsx
import React from 'react';

interface TextProps {
  children: React.ReactNode;
  style?: React.CSSProperties;
}

const Text: React.FC<TextProps> = ({ children, style }) => {
  return <p style={style}>{children}</p>;
};

interface VStackProps {
  children: React.ReactNode;
  spacing?: number;
  style?: React.CSSProperties;
}

const VStack: React.FC<VStackProps> = ({ children, spacing = 8, style }) => {
  const stackStyle: React.CSSProperties = {
    display: 'flex',
    flexDirection: 'column',
    gap: `${spacing}px`,
    ...style,
  };
  return <div style={stackStyle}>{children}</div>;
};

// Example usage:
// <VStack spacing={16}>
//   <Text>Hello, World!</Text>
//   <Text>This is a stack of text components.</Text>
// </VStack>
```

**[View on GitHub](https://github.com/your-username/your-repo/path/to/ui-components)**
