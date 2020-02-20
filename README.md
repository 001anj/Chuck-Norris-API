# Chuck-Norris-API
## API test for Chuck-Norris-API website using Postman/newman

### Steps to run the collections
1. Create a repository in Github named "Marvel-API" and clone it to your local directory
2. Install Postman and import the collection "Chucknorris_API_TEST" from test folder of repo into Postman.
3. Install the dependencies mentioned in package.JSON file.
4. Create a json file by running the command "npm init" in cmd while in same project directory
5. Change the line scripts with following line "test": "newman run test/Chucknorris_API_TEST.postman_collection.json"
6. Create a folder "test" inside your project directory and copy the Chucknorris_API_TEST.postman_collection.json in it.
7. Push the changes to GitHub (exclude node_modules files).

### Integration with CircleCI
1. Create a folder .circleci with file config.yml. For more information (https://devexpress.github.io/testcafe/documentation/continuous-integration/circleci.html)
2. Replace the text of config.yml with mentioned in this repository.
3. Log in to CircleCI using your GitHub account. If this is the first time you are using CircleCI, you will start from an empty workspace. Add the following project "Chuck-Norris-API" in it.
4. **Make sure that "Allow Uncertified Orbs" is enabled for the repository. Option can be found: CircleCI settings->security settings->check the option "Yes, allow all members of my organization to publish dev orbs, use uncertified orbs, and use third-party orbs (not supported by CircleCI) in project configuration.".
5. Click on button "start building" to trigger a build.
6. Check the test results.

