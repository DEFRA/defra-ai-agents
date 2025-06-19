# Defra AI Agents Playbook
This is a repository for the Defra AI Agents Playbook, which provides guidance on how to decide whether a use case is a good fit.

## Viewing the Playbook

The guide is best viewed in GitHub pages at https://github.com/DEFRA/defra-ai-agents/.

## Updating the Playbook

This documentation is written in markdown and is built using Jekyll.

### Updating the Playbook Locally
To update the playbook locally, you will need to ensure the following pre-requisites are met and then follow the steps to build and serve the playbook.

### Pre-requisites
Ruby (version 2.7 or later) - We recommend using a version manager like rbenv and ruby-build to install Ruby.

Bundler - Install it with gem install bundler.

### Building the Playbook

To build and update the playbook, follow these steps:

#### Clone the repository:

```
git clone https://github.com/DEFRA/defra-ai-agents
```


#### Navigate to the repository directory:

```
cd defra-ai-legacy-modernisation/playbook
```

#### Install the required gems:

```
bundle install
```

#### Build the site:

```
bundle exec jekyll build
```

#### Serve the site locally to preview changes:

```
bundle exec jekyll serve
```

Open your web browser and navigate to http://localhost:4000/defra-ai-agents/playbook to view the playbook.

## Licence
THIS INFORMATION IS LICENSED UNDER THE CONDITIONS OF THE OPEN GOVERNMENT LICENCE found at:

http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3

The following attribution statement MUST be cited in your products and applications when using this information.

Contains public sector information licensed under the Open Government license v3

### About the licence
The Open Government Licence (OGL) was developed by the Controller of Her Majesty's Stationery Office (HMSO) to enable information providers in the public sector to license the use and re-use of their information under a common open licence.

It is designed to encourage use and re-use of information freely and flexibly, with only a few conditions.