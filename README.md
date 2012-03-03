CodeIgniter GitHub Updater
===============================

This library is meant to handle updates to remote CodeIgniter instances. These updates 
are tied to a GitHub repository. Any time the repository is updated you can run the 
update command of this library to have your CodeIgniter files updated to the current 
version of the repository.

For more information check out my blog.

http://jimdoescode.blogspot.com/2012/02/keep-your-ci-instances-up-to-date-with.html

You can also see the test repo I use for performing remote updates.

https://github.com/jimdoescode/Test-Auto-Updater

Pay close attention to the welcome controller and the github_updater config file.

The ideal application would have several separate instances hosted by different parties like a CMS. Using this library you can create an upgrade script that will occasionally check if there is a new version available and perform updates when there is. That way users will never need to FTP updated files to their servers in order to stay up with the current version of your CI app. 

Usage
------
Copy the files under your application directory. 

Edit the github_updater.php config file.

Then load the library like this:

$this->load->library('github_updater');

$success = $this->github_updater->update();
		
License
-------
This library is licensed under the MIT license. 

