CloudFormation support for Visual Studio Code 
===================

This is fork of [ST3 CloudFormation plugin](https://github.com/beaknit/cform).


Usage
-------------

 1. Install the extension
 2. Create **new file**
 3. Set syntax to **JSON**
 4. Type **start** and press ```tab``` key to populate basic template skeleton
 5. **Start typing** desired **resource name** and hit ```tab``` key


> **Note:** CloudFormation support works with JSON syntax selected or .json, .cform, .template file extensions. These are commonly used CloudFormation template extensions.

![New template file](https://raw.githubusercontent.com/aws-scripting-guy/cform-VSCode/master/assets/new_template_file.gif)


YAML support
-------------------

YAML template creation follows the same syntax rules: type **start** to populate new template. Handsome of the most used snippets was translated. E.g.```s3-bucket```,```ec2-instance```,```rds-instance```,```elastic-load-balancer-internal```,```vpc```.

Please make sure you update regularly as additional snippets are being continuosly added.

Installation
-------------------

 1. Install Visual Studio Code 0.10.6 or higher
 2. Launch Code
 3. Invoke command palette by ```Ctrl-Shift-P``` (Windows, Linux) or ```Cmd-Shift-P``` (OSX)
 4. **Type** ```Extension```
 4. **Select** ```Install Extension```
 5. **Choose** extension **CloudFormation**
 6. Restart Visual Studio Code

![Installation](https://raw.githubusercontent.com/aws-scripting-guy/cform-VSCode/master/assets/install_extension.gif)

Troubleshooting
-------------------

* Users behing proxy: 
Download  **cform-latest.vsix** file from GitHub repo for manual install
[https://github.com/aws-scripting-guy/cform-VSCode](https://github.com/aws-scripting-guy/cform-VSCode)

Known issues
-------------------

When working with YAML documents, your current YAML language interpreter might not support syntax of AWS intrinsic functions, thus marking them as *unknown tag*. 
This however has no effect on validity of the YAML document. 

![YAML known issue](https://raw.githubusercontent.com/aws-scripting-guy/cform-VSCode/master/assets/known_issue1.png)

Changelog
-------------------
0.0.13
* yaml - most of the snippets translated 

0.0.12
* yaml - several new snippets added (vpc, ec2-instance, autoscaling-group, rds-dbinstance, elastic-load-balancer-internal, subnet, s3-bucket, s3-bucket-policy, cloudwatch-alarm, ref, get-azs,get-attr, parameter, output, map, find-in-map) 

0.0.11
* yaml - added experimental support 
* merged new snippets (Codepipeline, Codecommit, LaunchTemplate)
* corrected Tags property

0.0.10
* start snippet correction
* lambda support
* function IF

0.0.8
* corrected issue with missing language mode UI
* added latest .vsix to GitHub repo for manual install

0.0.6
* added support for .cform and .template file extensions

Contributing
-------------------

1. Fork
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -am 'Add some feature')
4. Push to the branch (git push origin my-new-feature)
5. Create new Pull Request

Donations appreciated :)
-------------------

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=5DE3L7KRM6RB8&lc=US&item_name=AWS%20Scripting%20Guy&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donate_LG%2egif%3aNonHosted)

