# slack-repo

A DNF/YUM repository for installing Slack on RHEL, CentOS, and Fedora Linux.

You can use the slack-repo RPM from [Copr](https://copr.fedorainfracloud.org/coprs/jdoss/slack-repo/) or you can drop the slack.repo file from this repository into `/etc/yum.repos.d` to enable it. From there, you can run `sudo dnf install slack` or `sudo yum install slack` to install the Slack for Linux client from Slack's [packagecloud](https://packagecloud.io/slacktechnologies/slack/) yum repository to enjoy automatic GPG verified RPM package updates.

**Why should I use this repository?**

Slack doesn't offer an official repo to use off of their Linux download page. This makes updating the Slack Linux client a manual process, with zero automatic GPG check on the RPM package you are about to install. Also, the install [instructions](https://packagecloud.io/slacktechnologies/slack/install#bash-rpm) on their packagecloud account will give you a repository for automatic package updates, but it uses an invalid GPG key which is less than helpful.

TL;DR: Having automatic Slack for Linux package updates and verifying the GPG signature on the RPM are possible if you use this repo. Yayy!

# License

MIT License

Copyright (c) 2018 Joe Doss

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
