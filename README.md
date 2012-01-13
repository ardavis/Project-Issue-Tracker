# School Manager Issue Tracker

The School Manager is a Ruby on Rails application developed by Andrew Davis hoping to improve the process of managing all of our many homework assignments/projects.

# Writing Issues

You can get to the [Issues](https://github.com/ardavis/Project-Issue-Tracker/issues) by clicking the link at the top of this page. When writing an issue, please choose an appropriate label. Issues can contain multiple labels, so if you feel it fits more than one, do so.

## Bug

If you notice a drastic issue with the application, such as numbers are incorrect, or broken pages are appearing, please file your issue under 'Bug'.

## Design

If you think you have an idea for re-designing a portion, or coming up with a new design piece, please write it under this label. If you can think of new associations between objects (such as how a user has many projects, and a school has many students, etc) please jot down all of your ideas.

## Feature

This is one of the most important to me as a developer. Features are anything that makes the application better. Example, if you want to add a course to a particular project, you could write this up as a 'Feature' for me to implement. Features follow this style:

    Feature: Add Course to Project
      In order to ensure I know what course my project is related to
      As a user
      I want to add a course to a project

      Background:
        Given I am a logged in user
        And I am on the home page
        And the following projects exist:
          | Title                           | Description                               |
          | Create a Smartphone Application | Make an app that does really cool things! |
        And the following courses exist:
          | Name                                    | Code   | Section |
          | Intro to Mobile Application Development | CE-491 | 01      |

      Scenario: Add a Course to a Project
        When I go to the project page
        And I attach the project to an existing course
        Then the project should be linked to the course

## Style

If you see something that looks funny, or you have ideas about improving the look and feel of the website, please classify the Issue under 'Style'.


