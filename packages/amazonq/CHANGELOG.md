## 1.14.0 2024-07-11

- **Feature** Amazon Q/dev proactively show code generation iterations

## 1.13.0 2024-07-11

- **Bug Fix** AD/LDAP users may see "uv_os_get_passwd ENOENT" error on startup #5277
- **Feature** Add support for [Amazon Q Chat Workspace Context](https://docs.aws.amazon.com/amazonq/latest/qdeveloper-ug/workspace-context.html). Customers can use `@workspace` to ask questions regarding local workspace.

## 1.12.0 2024-07-08

- **Bug Fix** Amazon Q Security Scans: Fixed unnecessary yellow lines appearing in both auto scans and project scans.
- **Bug Fix** Amazon Q Chat: Fixed prompt input becomes invisible if an html special character is inserted
- **Bug Fix** Amazon Q Chat: Fixed button font sizes are too big
- **Bug Fix** Amazon Q Chat: Fixed buttons don't show borders inside a message
- **Bug Fix** Amazon Q Code Transform: Link UI messages to troubleshooting docs
- **Bug Fix** Amazon Q /dev command: improve user error messages
- **Bug Fix** Amazon Q Chat: Fixed button texts are cropped too short
- **Bug Fix** Amazon Q Chat: Fixed prompt input and selected command horizontal alignment
- **Bug Fix** Amazon Q Chat: Fixed prompt input becomes invisible when multine text inserted with paste
- **Feature** Q feature dev: Only use relevant code and related files

## 1.11.0 2024-06-27

- **Bug Fix** Amazon Q Chat: Fix for inline buttons don't have borders
- **Bug Fix** Amazon Q Chat: Fix for some edge cases when followups appear on top without styles
- **Bug Fix** Amazon Q Chat: Fix for prompt input removes whole word if it starts with @ character but there is no context selected
- **Bug Fix** Amazon Q Chat: Fix for prompt input doesn't show multi line content properly after it reaches 10-15 lines
- **Bug Fix** Amazon Q /dev command: Fix in progress experience for ongoing backend calls

## 1.10.0 2024-06-21

- **Bug Fix** Security Scan: Fixes an issue where project-scans time out for larger projects.
- **Bug Fix** Amazon Q /dev command: Fix file rejections for files outside of src/
- **Bug Fix** Feature Development: update /dev welcome message
- **Bug Fix** Amazon Q Chat: Fixed broken code blocks with typewriter text in list items.
- **Feature** UX: New style for the login window
- **Removal** Auth: No longer share SSO sessions with AWS Toolkit.

## 1.9.0 2024-06-14

- **Bug Fix** Amazon Q inline suggestions: remember `Pause Auto-Suggestions` after IDE restart
- **Bug Fix** Amazon Q /dev command: stop showing spinner when there is an error.
- **Bug Fix** Security Scan: Fixes an issue where auto-scans cause the editor to become unresponsive for larger projects.
- **Bug Fix** Fix(Amazon Q Code Transformation): show more detailed error messages for proxy issues
- **Feature** Amazon Q Code Transform: Allow user to view transformation build log

## 1.8.0 2024-06-07

- **Bug Fix** fix(featureDev): fix file rejection for multi-workspaces
- **Feature** The `Send to Amazon Q` [context menu](https://github.com/aws/aws-toolkit-vscode/assets/371007/ce4c61a4-1b58-48ee-8500-56667d45dd7d) was renamed to `Amazon Q`
- **Feature** Amazon Q Transform: Increase project upload size limit to 2GB
- **Feature** feat(featureDev): generated plan being shown from top
- **Feature** Add additional commands for Amazon Q.

## 1.7.0 2024-05-30

- **Bug Fix** Feature Development: File rejection is not rejecting a file when code is generated
- **Bug Fix** Security Scan: Improved accuracy when applying security fixes
- **Bug Fix** Amazon Q Code Transformation: show more specific error messages on failure cases
- **Feature** Security Scan: Support for scanning files outside of workspaces.
- **Feature** Amazon Q now publishes to Open VSX: https://open-vsx.org/namespace/amazonwebservices

## 1.6.0 2024-05-21

- **Bug Fix** Amazon Q Chat: Inside chat body, if there is a code block inside a list item it shows <br/> tags
- **Bug Fix** Amazon Q Chat: Prompt input field allows additional input beyond the character limit
- **Bug Fix** Amazon Q Chat: Prompt input field not getting focus when chat window opens

## 1.5.0 2024-05-17

- **Bug Fix** Security Scan: Fixes an issue when scanning projects with binary files
- **Bug Fix** Fixes an issue where the /dev chat wouldn't let customers modify the source folder when exceeding the size limit
- **Bug Fix** Security Scan: Improved error notifications
- **Feature** Security Scan: Added custom command to run the security scan.
- **Feature** Security Scan: "View details" and "Explain" options can now be accessed from the problems panel

## 1.4.0 2024-05-13

- **Bug Fix** Auth: No longer request AWS account scopes during login.
- **Bug Fix** Security Scan: Fixes an issue where scans fail for projects with Terraform files
- **Bug Fix** Amazon Q Code Transform: Show additional status messages to align with experience when JAVA_HOME set incorrectly.
- **Feature** UX: Added keyboard navigation to login screen.
- **Feature** New SSO Authorization Code flow for faster logins
- **Feature** Transform: Add human intervention to help update dependencies during transformation.

## 1.3.0 2024-05-08

- **Bug Fix** modifying the root folder for /dev now modifies it
- **Bug Fix** Q chat may stop responding after processing Javascript/Typescript code
- **Bug Fix** Completion may fail unexpected if user opened many tabs
- **Feature** Inline Suggestions: Only display the 'Open Chat' CodeLens if the user is signed into Amazon Q.
- **Feature** Security Scan: Scans can now be run without an open editor
- **Feature** Security Scan: Multi-root workspace support

## 1.2.0 2024-05-07

- **Bug Fix** Fix bug when Amazon Q chat sends code selection while user has no selection
- **Bug Fix** Amazon Q Code Transformation: make jobId visible in job history tab at start of job and allow summary.md + icons to be saved when accepting changes
- **Bug Fix** Amazon Q Chat: Typewriter animator parts showing up in code fields inside listitems
- **Bug Fix** Security Scan: Addresses a bug where security issues sometimes appear multiple times
- **Feature** Update cross file context config for Q inline suggestion
- **Feature** Amazon Q: Security scans now support C, C++, and PHP files

## 1.1.0 2024-04-30

- **Bug Fix** Amazon Q Chat: Fixed markdown is not getting parsed inside list items.
- **Bug Fix** Amazon Q Chat: Copy to clipboard on code blocks doesn't work
- **Bug Fix** Fixed a crash when trying to use Q /dev on large projects or projects containing files with unsupported encoding.

## 1.0.0 2024-04-29

- **Bug Fix** Code Transformation: Address various issues in TransformationHub UX.
- **Bug Fix** Code Transformation: Transform may fail if JAVA_HOME has leading or trailing whitespace
- **Bug Fix** Chat: Q panel doesn't fit to its parent
- **Bug Fix** Feature Development: update welcome message and menu item description for /dev command
- **Bug Fix** Code Transformation: show error messages in chat
- **Bug Fix** Code Transformation: Proposed changes not updated when multiple transformation jobs run in sequence.
- **Bug Fix** Feature Development: Update error message for monthly conversation limit reach
- **Bug Fix** Code Transformation: Omit Maven metadata files when uploading dependencies to fix certain build failures in backend.
- **Feature** Code Transformation: Refreshed UI during CodeTransformation
- **Feature** Chat: cmd + i to open chat
- **Feature** Right Click + no code selected shows Q context menu
- **Feature** Security Scan: Scans can now run on all files in the project
- **Feature** Chat: Updates quick action commands style and groupings
- **Feature** Code Transformation: add details about expected changes in transformation plan
- **Feature** Enable Amazon Q feature development and Amazon Q transform capabilities (/dev and /transform) for AWS Builder ID users.
- **Feature** Initial release
- **Feature** Chat: Added metric parameters to recordAddMessage telemetry event.
- **Feature** Security Scan: Scans can now run automatically when file changes are made
- **Feature** Chat: brief CodeLens to advertise chat
- **Feature** Security Scan: Send security issue to chat for explanation and fix

