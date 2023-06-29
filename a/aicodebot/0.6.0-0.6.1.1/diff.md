# Comparing `tmp/aicodebot-0.6.0.tar.gz` & `tmp/aicodebot-0.6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.6.0.tar", last modified: Tue Jun 27 20:55:28 2023, max compression
+gzip compressed data, was "aicodebot-0.6.1.1.tar", last modified: Thu Jun 29 15:20:34 2023, max compression
```

## Comparing `aicodebot-0.6.0.tar` & `aicodebot-0.6.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:55:28.348593 aicodebot-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 20:54:57.000000 aicodebot-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-06-27 20:55:28.348593 aicodebot-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-06-27 20:54:57.000000 aicodebot-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:55:28.344593 aicodebot-0.6.0/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-27 20:54:57.000000 aicodebot-0.6.0/aicodebot/.aicodebot.template
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 20:54:57.000000 aicodebot-0.6.0/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-06-27 20:54:57.000000 aicodebot-0.6.0/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-27 20:54:57.000000 aicodebot-0.6.0/aicodebot/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:55:28.348593 aicodebot-0.6.0/aicodebot/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 20:54:57.000000 aicodebot-0.6.0/aicodebot/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-27 20:54:57.000000 aicodebot-0.6.0/aicodebot/prompts/alignment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-27 20:54:57.000000 aicodebot-0.6.0/aicodebot/prompts/commit_message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 20:54:57.000000 aicodebot-0.6.0/aicodebot/prompts/debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-27 20:54:57.000000 aicodebot-0.6.0/aicodebot/prompts/fun_fact.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-27 20:54:57.000000 aicodebot-0.6.0/aicodebot/prompts/review.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:55:28.348593 aicodebot-0.6.0/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-06-27 20:55:28.000000 aicodebot-0.6.0/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 20:55:28.000000 aicodebot-0.6.0/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 20:55:28.000000 aicodebot-0.6.0/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 20:55:28.000000 aicodebot-0.6.0/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-27 20:55:28.000000 aicodebot-0.6.0/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 20:55:28.000000 aicodebot-0.6.0/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-27 20:54:57.000000 aicodebot-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 20:55:28.348593 aicodebot-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-27 20:54:57.000000 aicodebot-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:20:34.054724 aicodebot-0.6.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-06-29 15:20:34.054724 aicodebot-0.6.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:20:34.050724 aicodebot-0.6.1.1/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/.aicodebot.template
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:20:34.054724 aicodebot-0.6.1.1/aicodebot/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/prompts/alignment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/prompts/commit_message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/prompts/debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/prompts/fun_fact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/prompts/review.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:20:34.050724 aicodebot-0.6.1.1/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-06-29 15:20:34.000000 aicodebot-0.6.1.1/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-29 15:20:34.000000 aicodebot-0.6.1.1/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:20:34.000000 aicodebot-0.6.1.1/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 15:20:34.000000 aicodebot-0.6.1.1/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:20:34.000000 aicodebot-0.6.1.1/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 15:20:34.000000 aicodebot-0.6.1.1/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:20:34.054724 aicodebot-0.6.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/setup.py
```

### Comparing `aicodebot-0.6.0/LICENSE` & `aicodebot-0.6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.0/PKG-INFO` & `aicodebot-0.6.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: aicodebot
-Version: 0.6.0
-Summary: Your AI-powered coding companion: AI Code Bot 🤖
-Home-page: https://github.com/novara_ai/aicodebot
-Author: Nick Sullivan
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # AI Code Bot 🤖
 
 ## Your AI-powered coding companion
 
 AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer - a team member that accelerates the pace of development and helps you write better code.
 
 There are lot of ways to use AICodeBot that we have planned. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
@@ -35,23 +18,39 @@
 
 It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, AICodeBot is built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
 ## Current features - how you can use it
 
 ### AI-Assisted Git Commit
 
-`aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. It will also commit the changes for you once everything checks out.
+`aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that describes the change. It will also commit the changes for you once everything checks out.
+
+### AI-Assisted Code Review
+
+`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It's goal is to suggest how to make the code better, and we've found that it often teaches us new things about our code. It's not perfect, but it's a great way to get a second set of robot eyes on your code.
 
 ### AI-Assisted Debugging
 
-`aicodebot debug $command` will run the command and capture the log message. It will then try to figure out what's going on from the error message and suggest a fix.
+`aicodebot debug $command` will run the command and capture the log message. It will pass the error message, stack trace, comand output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to stackoverflow in a separate window, allowing you to stay in terminal with all the context.
 
-### AI-Assisted Code Review
+### AI-Assisted Code Creation (Work in Progress)
+
+`aicodebot code` is a feature designed to automate coding tasks based on your instructions. It's a work in progress, but here's how it works:
+
+1. **Task Understanding**: The bot collects your task instructions.
+2. **Planning**: It devises a plan based on your task.
+3. **Learning**: It learns necessary information by searching the internet, reading the local codebase, and researching libraries/APIs.
+4. **Clarification**: It asks questions if any aspect of the task is unclear.
+5. **Code Generation**: It generates code consistent with your codebase style.
+6. **Self-Review**: It reviews and improves the generated code.
+7. **Code Modification**: It modifies the local code, allowing you to review changes before committing.
+8. **Test Creation**: It writes and runs unit tests for the new code, modifying the code until all tests pass.
+9. **Continuous Learning (v2)**: We plan to implement a system where the bot learns from each interaction, improving its performance over time based on feedback like code acceptance, compilation success, and test results.
 
-`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It also suggests best practices for code improvement.
+This feature is a work in progress, and we're excited about its potential to boost developer productivity. If you'd like to help, see [CONTRIBUTING](CONTRIBUTING.md).
 
 ## Getting Started
 
 [![PyPI version](https://badge.fury.io/py/aicodebot.svg)](https://badge.fury.io/py/aicodebot)
 
 To install AICodeBot, run:
 
@@ -84,49 +83,50 @@
 
 Not all OpenAI accounts have GPT-4 API access enabled. By default, AICodeBot will use GPT-4 if your OpenAI account supports it, we will check the first time you run it. Tip: If your OpenAI API does not support GPT-4, you can ask to be added to the waitlist [here](https://openai.com/waitlist/gpt-4-api)
 
 ## Roadmap of Upcoming Features
 
 ### Code Workflow Improvements
 
-- [X] **Assisted Git Commit**: Automatically generate a commit message based on the changes you've made
-- [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
-- [X] **Code Review**: Provides feedback on potential issues in code,  and suggests improvements to make it better.
-- [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
-- [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
-- [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
-- [ ] **Test Generation**: Generates unit tests for code, improve test coverage.
-- [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions). Eventually: Fix the build automatically when there are small errors.
-- [ ] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems, using data from the current repository.
-- [X] **Linting/Formatting**: Checks code for linting errors and automatically fixes them where possible (via pre-commit)
-- [ ] **Handle GitHub Issues**: Handles basic tasks that you assign to [@aicodebot](https://pypi.org/project/aicodebot/)
+* [X] **Assisted Git Commit**: Automatically generate a commit message based on the changes you've made
+* [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
+* [X] **Code Review**: Provides feedback on potential issues in code,  and suggests improvements to make it better.
+* [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
+* [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
+* [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
+* [ ] **Test Generation**: Generates unit tests for code, improve test coverage.
+* [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions). Eventually: Fix the build automatically when there are small errors.
+* [ ] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems, using data from the current repository.
+* [X] **Linting/Formatting**: Checks code for linting errors and automatically fixes them where possible (via pre-commit)
+* [ ] **Handle GitHub Issues**: Handles basic tasks that you assign to [@aicodebot](https://pypi.org/project/aicodebot/)
+* [ ] **Automatically Generate ChangeLogs and Release Notes**: Generates release notes and changelogs based on commit messages and code changes.
 
 ### User Interfaces
 
-- [X] **Command-line, installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
-- [ ] **Mention the @aicodebot GitHub user**: Mentioning the [@aicodebot](https://pypi.org/project/aicodebot/) GitHub user in a comment will trigger it to perform a task, review code, or pull in an appropriate GIF.
-- [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
-- [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
-- [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
-- [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
+* [X] **Command-line, installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
+* [ ] **Mention the @aicodebot GitHub user**: Mentioning the [@aicodebot](https://pypi.org/project/aicodebot/) GitHub user in a comment will trigger it to perform a task, review code, or pull in an appropriate GIF.
+* [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
+* [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
+* [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
+* [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
 
 ### Repository Management
 
-- [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
-- [ ] **Handle Stale Issues**: Automatically detects and handles stale issues on GitHub by nudging the responsible parties.
-- [ ] **Triage Incoming Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary.
-- [ ] **Rate the complexity of PRs**: Rates the complexity of pull requests and assigns them to developers based on their skill level and context
+* [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
+* [ ] **Handle Stale Issues**: Automatically detects and handles stale issues on GitHub by nudging the responsible parties.
+* [ ] **Triage Incoming Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary.
+* [ ] **Rate the complexity of PRs**: Rates the complexity of pull requests and assigns them to developers based on their skill level and context
 
 ### Fun
 
-- [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming. Try it out with `aicodebot fun-fact`.
-- [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity. Try it out with `aicodebot alignment`.
-- [ ] **Telling Jokes**: We've gotta figure out how to teach LLMs about humor. :)
-- [ ] **Supportive Encouragement**: High fives and kudos for a job well done
-- [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs.
+* [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming. Try it out with `aicodebot fun-fact`.
+* [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity. Try it out with `aicodebot alignment`.
+* [ ] **Telling Jokes**: We've gotta figure out how to teach LLMs about humor. :)
+* [ ] **Supportive Encouragement**: High fives and kudos for a job well done
+* [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs.
 
 <img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" width="25%">
 
 ## Alignment ❤️ + 🤖
 
 Technology itself is amoral, it just imbues the values of the engineers who create it. We believe that AI should be built-in a way that aligns with humanity, and we're building aicodebot to help us do just that. We're building from a heart-centered space, and contributing to the healthy intersection of AI and humanity.
```

### Comparing `aicodebot-0.6.0/README.md` & `aicodebot-0.6.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: aicodebot
+Version: 0.6.1.1
+Summary: Your AI-powered coding companion: AI Code Bot 🤖
+Home-page: https://github.com/novara_ai/aicodebot
+Author: Nick Sullivan
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # AI Code Bot 🤖
 
 ## Your AI-powered coding companion
 
 AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer - a team member that accelerates the pace of development and helps you write better code.
 
 There are lot of ways to use AICodeBot that we have planned. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
@@ -18,23 +35,39 @@
 
 It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, AICodeBot is built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
 ## Current features - how you can use it
 
 ### AI-Assisted Git Commit
 
-`aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. It will also commit the changes for you once everything checks out.
+`aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that describes the change. It will also commit the changes for you once everything checks out.
+
+### AI-Assisted Code Review
+
+`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It's goal is to suggest how to make the code better, and we've found that it often teaches us new things about our code. It's not perfect, but it's a great way to get a second set of robot eyes on your code.
 
 ### AI-Assisted Debugging
 
-`aicodebot debug $command` will run the command and capture the log message. It will then try to figure out what's going on from the error message and suggest a fix.
+`aicodebot debug $command` will run the command and capture the log message. It will pass the error message, stack trace, comand output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to stackoverflow in a separate window, allowing you to stay in terminal with all the context.
 
-### AI-Assisted Code Review
+### AI-Assisted Code Creation (Work in Progress)
+
+`aicodebot code` is a feature designed to automate coding tasks based on your instructions. It's a work in progress, but here's how it works:
+
+1. **Task Understanding**: The bot collects your task instructions.
+2. **Planning**: It devises a plan based on your task.
+3. **Learning**: It learns necessary information by searching the internet, reading the local codebase, and researching libraries/APIs.
+4. **Clarification**: It asks questions if any aspect of the task is unclear.
+5. **Code Generation**: It generates code consistent with your codebase style.
+6. **Self-Review**: It reviews and improves the generated code.
+7. **Code Modification**: It modifies the local code, allowing you to review changes before committing.
+8. **Test Creation**: It writes and runs unit tests for the new code, modifying the code until all tests pass.
+9. **Continuous Learning (v2)**: We plan to implement a system where the bot learns from each interaction, improving its performance over time based on feedback like code acceptance, compilation success, and test results.
 
-`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It also suggests best practices for code improvement.
+This feature is a work in progress, and we're excited about its potential to boost developer productivity. If you'd like to help, see [CONTRIBUTING](CONTRIBUTING.md).
 
 ## Getting Started
 
 [![PyPI version](https://badge.fury.io/py/aicodebot.svg)](https://badge.fury.io/py/aicodebot)
 
 To install AICodeBot, run:
 
@@ -67,49 +100,50 @@
 
 Not all OpenAI accounts have GPT-4 API access enabled. By default, AICodeBot will use GPT-4 if your OpenAI account supports it, we will check the first time you run it. Tip: If your OpenAI API does not support GPT-4, you can ask to be added to the waitlist [here](https://openai.com/waitlist/gpt-4-api)
 
 ## Roadmap of Upcoming Features
 
 ### Code Workflow Improvements
 
-- [X] **Assisted Git Commit**: Automatically generate a commit message based on the changes you've made
-- [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
-- [X] **Code Review**: Provides feedback on potential issues in code,  and suggests improvements to make it better.
-- [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
-- [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
-- [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
-- [ ] **Test Generation**: Generates unit tests for code, improve test coverage.
-- [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions). Eventually: Fix the build automatically when there are small errors.
-- [ ] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems, using data from the current repository.
-- [X] **Linting/Formatting**: Checks code for linting errors and automatically fixes them where possible (via pre-commit)
-- [ ] **Handle GitHub Issues**: Handles basic tasks that you assign to [@aicodebot](https://pypi.org/project/aicodebot/)
+* [X] **Assisted Git Commit**: Automatically generate a commit message based on the changes you've made
+* [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
+* [X] **Code Review**: Provides feedback on potential issues in code,  and suggests improvements to make it better.
+* [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
+* [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
+* [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
+* [ ] **Test Generation**: Generates unit tests for code, improve test coverage.
+* [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions). Eventually: Fix the build automatically when there are small errors.
+* [ ] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems, using data from the current repository.
+* [X] **Linting/Formatting**: Checks code for linting errors and automatically fixes them where possible (via pre-commit)
+* [ ] **Handle GitHub Issues**: Handles basic tasks that you assign to [@aicodebot](https://pypi.org/project/aicodebot/)
+* [ ] **Automatically Generate ChangeLogs and Release Notes**: Generates release notes and changelogs based on commit messages and code changes.
 
 ### User Interfaces
 
-- [X] **Command-line, installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
-- [ ] **Mention the @aicodebot GitHub user**: Mentioning the [@aicodebot](https://pypi.org/project/aicodebot/) GitHub user in a comment will trigger it to perform a task, review code, or pull in an appropriate GIF.
-- [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
-- [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
-- [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
-- [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
+* [X] **Command-line, installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
+* [ ] **Mention the @aicodebot GitHub user**: Mentioning the [@aicodebot](https://pypi.org/project/aicodebot/) GitHub user in a comment will trigger it to perform a task, review code, or pull in an appropriate GIF.
+* [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
+* [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
+* [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
+* [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
 
 ### Repository Management
 
-- [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
-- [ ] **Handle Stale Issues**: Automatically detects and handles stale issues on GitHub by nudging the responsible parties.
-- [ ] **Triage Incoming Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary.
-- [ ] **Rate the complexity of PRs**: Rates the complexity of pull requests and assigns them to developers based on their skill level and context
+* [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
+* [ ] **Handle Stale Issues**: Automatically detects and handles stale issues on GitHub by nudging the responsible parties.
+* [ ] **Triage Incoming Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary.
+* [ ] **Rate the complexity of PRs**: Rates the complexity of pull requests and assigns them to developers based on their skill level and context
 
 ### Fun
 
-- [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming. Try it out with `aicodebot fun-fact`.
-- [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity. Try it out with `aicodebot alignment`.
-- [ ] **Telling Jokes**: We've gotta figure out how to teach LLMs about humor. :)
-- [ ] **Supportive Encouragement**: High fives and kudos for a job well done
-- [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs.
+* [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming. Try it out with `aicodebot fun-fact`.
+* [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity. Try it out with `aicodebot alignment`.
+* [ ] **Telling Jokes**: We've gotta figure out how to teach LLMs about humor. :)
+* [ ] **Supportive Encouragement**: High fives and kudos for a job well done
+* [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs.
 
 <img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" width="25%">
 
 ## Alignment ❤️ + 🤖
 
 Technology itself is amoral, it just imbues the values of the engineers who create it. We believe that AI should be built-in a way that aligns with humanity, and we're building aicodebot to help us do just that. We're building from a heart-centered space, and contributing to the healthy intersection of AI and humanity.
```

### Comparing `aicodebot-0.6.0/aicodebot/cli.py` & `aicodebot-0.6.1.1/aicodebot/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pathlib import Path
 from rich.console import Console
 from rich.style import Style
 import click, datetime, openai, os, random, subprocess, sys, tempfile, webbrowser
 
 # ----------------------------- Default settings ----------------------------- #
 
-DEFAULT_MAX_TOKENS = 1024
+DEFAULT_MAX_TOKENS = 512
 DEFAULT_TEMPERATURE = 0.1
 DEFAULT_SPINNER = "point"
 
 # ----------------------- Setup for rich console output ---------------------- #
 console = Console()
 bot_style = Style(color="#30D5C8")
 
@@ -302,14 +302,18 @@
     model_options = {
         "gpt-4": 8192,
         "gpt-4-32k": 32768,
         "gpt-3.5-turbo": 4096,
         "gpt-3.5-turbo-16k": 16384,
     }
     gpt_4_supported = os.getenv("GPT_4_SUPPORTED") == "true"
+
+    # For some unknown reason, tiktoken often underestimates the token size by ~10%, so let's buffer
+    token_size = int(token_size * 1.1)
+
     if gpt_4_supported:
         if token_size <= model_options["gpt-4"]:
             return "gpt-4"
         elif token_size <= model_options["gpt-4-32k"]:
             return "gpt-4-32k"
         else:
             raise click.ClickException("🛑 The context is too large to for the Model. 😞")
```

### Comparing `aicodebot-0.6.0/aicodebot/helpers.py` & `aicodebot-0.6.1.1/aicodebot/helpers.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.0/aicodebot/prompts/alignment.yaml` & `aicodebot-0.6.1.1/aicodebot/prompts/alignment.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.0/aicodebot/prompts/commit_message.yaml` & `aicodebot-0.6.1.1/aicodebot/prompts/commit_message.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.0/aicodebot/prompts/review.yaml` & `aicodebot-0.6.1.1/aicodebot/prompts/review.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.0/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.6.1.1/aicodebot.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.6.0
+Version: 0.6.1.1
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -35,23 +35,39 @@
 
 It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, AICodeBot is built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
 ## Current features - how you can use it
 
 ### AI-Assisted Git Commit
 
-`aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. It will also commit the changes for you once everything checks out.
+`aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that describes the change. It will also commit the changes for you once everything checks out.
+
+### AI-Assisted Code Review
+
+`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It's goal is to suggest how to make the code better, and we've found that it often teaches us new things about our code. It's not perfect, but it's a great way to get a second set of robot eyes on your code.
 
 ### AI-Assisted Debugging
 
-`aicodebot debug $command` will run the command and capture the log message. It will then try to figure out what's going on from the error message and suggest a fix.
+`aicodebot debug $command` will run the command and capture the log message. It will pass the error message, stack trace, comand output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to stackoverflow in a separate window, allowing you to stay in terminal with all the context.
 
-### AI-Assisted Code Review
+### AI-Assisted Code Creation (Work in Progress)
+
+`aicodebot code` is a feature designed to automate coding tasks based on your instructions. It's a work in progress, but here's how it works:
+
+1. **Task Understanding**: The bot collects your task instructions.
+2. **Planning**: It devises a plan based on your task.
+3. **Learning**: It learns necessary information by searching the internet, reading the local codebase, and researching libraries/APIs.
+4. **Clarification**: It asks questions if any aspect of the task is unclear.
+5. **Code Generation**: It generates code consistent with your codebase style.
+6. **Self-Review**: It reviews and improves the generated code.
+7. **Code Modification**: It modifies the local code, allowing you to review changes before committing.
+8. **Test Creation**: It writes and runs unit tests for the new code, modifying the code until all tests pass.
+9. **Continuous Learning (v2)**: We plan to implement a system where the bot learns from each interaction, improving its performance over time based on feedback like code acceptance, compilation success, and test results.
 
-`aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It also suggests best practices for code improvement.
+This feature is a work in progress, and we're excited about its potential to boost developer productivity. If you'd like to help, see [CONTRIBUTING](CONTRIBUTING.md).
 
 ## Getting Started
 
 [![PyPI version](https://badge.fury.io/py/aicodebot.svg)](https://badge.fury.io/py/aicodebot)
 
 To install AICodeBot, run:
 
@@ -84,49 +100,50 @@
 
 Not all OpenAI accounts have GPT-4 API access enabled. By default, AICodeBot will use GPT-4 if your OpenAI account supports it, we will check the first time you run it. Tip: If your OpenAI API does not support GPT-4, you can ask to be added to the waitlist [here](https://openai.com/waitlist/gpt-4-api)
 
 ## Roadmap of Upcoming Features
 
 ### Code Workflow Improvements
 
-- [X] **Assisted Git Commit**: Automatically generate a commit message based on the changes you've made
-- [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
-- [X] **Code Review**: Provides feedback on potential issues in code,  and suggests improvements to make it better.
-- [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
-- [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
-- [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
-- [ ] **Test Generation**: Generates unit tests for code, improve test coverage.
-- [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions). Eventually: Fix the build automatically when there are small errors.
-- [ ] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems, using data from the current repository.
-- [X] **Linting/Formatting**: Checks code for linting errors and automatically fixes them where possible (via pre-commit)
-- [ ] **Handle GitHub Issues**: Handles basic tasks that you assign to [@aicodebot](https://pypi.org/project/aicodebot/)
+* [X] **Assisted Git Commit**: Automatically generate a commit message based on the changes you've made
+* [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
+* [X] **Code Review**: Provides feedback on potential issues in code,  and suggests improvements to make it better.
+* [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
+* [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
+* [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
+* [ ] **Test Generation**: Generates unit tests for code, improve test coverage.
+* [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions). Eventually: Fix the build automatically when there are small errors.
+* [ ] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems, using data from the current repository.
+* [X] **Linting/Formatting**: Checks code for linting errors and automatically fixes them where possible (via pre-commit)
+* [ ] **Handle GitHub Issues**: Handles basic tasks that you assign to [@aicodebot](https://pypi.org/project/aicodebot/)
+* [ ] **Automatically Generate ChangeLogs and Release Notes**: Generates release notes and changelogs based on commit messages and code changes.
 
 ### User Interfaces
 
-- [X] **Command-line, installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
-- [ ] **Mention the @aicodebot GitHub user**: Mentioning the [@aicodebot](https://pypi.org/project/aicodebot/) GitHub user in a comment will trigger it to perform a task, review code, or pull in an appropriate GIF.
-- [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
-- [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
-- [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
-- [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
+* [X] **Command-line, installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
+* [ ] **Mention the @aicodebot GitHub user**: Mentioning the [@aicodebot](https://pypi.org/project/aicodebot/) GitHub user in a comment will trigger it to perform a task, review code, or pull in an appropriate GIF.
+* [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
+* [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
+* [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
+* [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
 
 ### Repository Management
 
-- [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
-- [ ] **Handle Stale Issues**: Automatically detects and handles stale issues on GitHub by nudging the responsible parties.
-- [ ] **Triage Incoming Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary.
-- [ ] **Rate the complexity of PRs**: Rates the complexity of pull requests and assigns them to developers based on their skill level and context
+* [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
+* [ ] **Handle Stale Issues**: Automatically detects and handles stale issues on GitHub by nudging the responsible parties.
+* [ ] **Triage Incoming Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary.
+* [ ] **Rate the complexity of PRs**: Rates the complexity of pull requests and assigns them to developers based on their skill level and context
 
 ### Fun
 
-- [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming. Try it out with `aicodebot fun-fact`.
-- [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity. Try it out with `aicodebot alignment`.
-- [ ] **Telling Jokes**: We've gotta figure out how to teach LLMs about humor. :)
-- [ ] **Supportive Encouragement**: High fives and kudos for a job well done
-- [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs.
+* [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming. Try it out with `aicodebot fun-fact`.
+* [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity. Try it out with `aicodebot alignment`.
+* [ ] **Telling Jokes**: We've gotta figure out how to teach LLMs about humor. :)
+* [ ] **Supportive Encouragement**: High fives and kudos for a job well done
+* [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs.
 
 <img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" width="25%">
 
 ## Alignment ❤️ + 🤖
 
 Technology itself is amoral, it just imbues the values of the engineers who create it. We believe that AI should be built-in a way that aligns with humanity, and we're building aicodebot to help us do just that. We're building from a heart-centered space, and contributing to the healthy intersection of AI and humanity.
```

### Comparing `aicodebot-0.6.0/aicodebot.egg-info/SOURCES.txt` & `aicodebot-0.6.1.1/aicodebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.0/pyproject.toml` & `aicodebot-0.6.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.0/setup.py` & `aicodebot-0.6.1.1/setup.py`

 * *Files identical despite different names*

