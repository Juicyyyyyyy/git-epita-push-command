# Git Epita Push

`git epita-push` is a custom Git command that automates the process of adding files, committing changes, creating annotated tags, and pushing both commits and tags to a remote Git repository.

## Installation

1. **Clone the Repository:**

   Clone this repository to your local machine:

   ```bash
   git clone https://github.com/Juicyyyyyyy/git-epita-push.git
   ```

2. **Navigate to the Directory:**

   ```bash
   cd git-epita-push
   ```

3. **Make the Script Executable:**

   Change the script's permissions to make it executable:

   ```bash
   chmod +x git-epita-push
   ```

4. **Move the Script to Your PATH:**

   Move the script to a directory in your PATH, such as `/usr/local/bin`:

   ```bash
   sudo mv git-epita-push /usr/local/bin/
   ```

## Usage

To use the `git epita-push` command, run:

```bash
git epita-push <tag-name> <message> [file-to-add]
```

### Arguments:

- `<tag-name>`: The base name of the tag you want to create.
- `<message>`: The commit and tag message.
- `[file-to-add]`: (Optional) The file to add. Defaults to `.` (all changes).

### Example:

1. To commit a specific file and create a tag:

   ```bash
   git epita-push this_is_a_tag_name "this_is_a_message" myfile.txt
   ```

2. To commit all changes and create a tag:

   ```bash
   git epita-push this_is_a_tag_name "this_is_a_message"
   ```

### Help

To display usage information and command details, run:

```bash
git epita-push -help
```
