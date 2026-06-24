Hands-on Lab: Git Tracking for a Simple Form (Lab Notes)
Task 1: Cloning the Repo
To start the project, I needed to get the files from my GitHub account down onto my laptop. I opened up the command prompt terminal on my Lenovo laptop, and used the file directory navigation to get into my school projects folder. After that, I typed in the cloning command to download everything.

git clone https://github.com/oginniisrael4-bot/simple-form.git

cd simple-form

The first command downloaded the whole setup from the internet, and then the second command shifted my terminal so I was actually working inside that new folder. If I didn't type that second command, none of my next steps would work because I'd be in the wrong directory.

Task 2 & 3: Adding the Files and Making the First Commit
Once the folder was ready on my computer, I opened up my normal file explorer and dragged the client's files, which were form.html and style.css, right into that project folder. Even though the files were inside the folder, Git wasn't watching them yet. They were untracked. To fix this, I had to stage them and save them.

git add form.html style.css

git commit -m "Initial commit for simple form"

The git add command put the files in a temporary waiting area, and the git commit command took a permanent snapshot of them. I added a small message inside the quotes so I can remember that this was my very first version.

Task 4: Pushing to GitHub
Right now, the save point I just created is only sitting on my laptop's hard drive. If something happens to my laptop, I'd lose all my work. To back it up safely on the cloud, I pushed the files up to my online GitHub repository profile under the main branch.

git push origin main

This sent everything up to the web, so now my online profile matches exactly what I have on my computer.

Task 5 & 6: Updating the Form (Adding Phone Number)
A bit later, the client sent an update saying they wanted to collect phone numbers too. I opened up form.html in my text editor, typed in the new input box tags for the phone number, and then opened up style.css to add some padding so the new box didn't look squeezed or messy. After checking that it looked okay on my screen, I staged and committed this new version, then pushed it online.

git add form.html style.css

git commit -m "Added phone number field and updated styles"

git push origin main

Now, the online GitHub repository has the updated version with the new phone number section.

Task 7 & 8: Checking History and Reverting a Bug
To see all the different versions and work I've done so far, I used the history log command.

git log

When I ran this, it showed a long list of my previous saves, along with the date, time, and those long strings of mixed letters and numbers called commit hashes.

Right after the update, the client complained that the form submission process was suddenly glitching out. Instead of panicking and trying to undo my code line by line, I looked at my log, found the long hash ID from my very first working version, and used it to roll just the HTML file back to how it was before the bug.

git checkout 4a2b3c1 -- form.html

That 4a2b3c1 code is just an example of the ID I copied from my terminal list. Running this instantly replaced my broken HTML file with the clean, original version.

Task 9 & 10: Testing a CAPTCHA on a New Branch
Next, the client wanted to test out a CAPTCHA security box to stop fake spam messages. Since this was just an experiment and I didn't want to break the form again, I decided to create a separate side workspace called a branch. I named it feature-add-captcha and jumped onto it.

git checkout -b feature-add-captcha

While working on this side branch, I added the CAPTCHA code and committed the change. The cool thing is that this save didn't touch my main, working website files at all.

git add form.html

git commit -m "Added CAPTCHA feature"

After testing it out and seeing that the CAPTCHA worked perfectly without causing any bugs, I switched back to my primary main branch, merged the side branch into it, and pushed the final result up to GitHub.

git checkout main

git merge feature-add-captcha

git push origin main

Task 11: Undoing a Mistake Locally
Later on, I was playing around with some colors inside style.css and completely messed up the design layout. It looked terrible, and I couldn't remember what the original numbers were. Since I hadn't made a commit save on these bad changes yet, I used a shortcut to completely wipe out my temporary mistakes and reset the file back to how it looked at my last safe commit.

git checkout -- style.css

This instantly brought back my clean layout and saved me from having to re-type everything.

Task 12: Pulling the Latest Updates
Lastly, just in case I ever make changes directly on the GitHub website using a browser, or if I start working with other people, I need to make sure my laptop has the newest files before I start typing. I used the pull command to fetch any online updates down to my computer.

git pull origin main

What I Learned From This Lab
Using commits is just like saving your progress in a video game. You can try out crazy ideas or edit whatever you want, and if things go completely wrong, you don't have to start over from scratch. You can just reload your last safe checkpoint using the commit log.

Branches are absolute lifesavers. Creating a side branch gives you a private sandbox to test new things. It keeps your main code line safe from breaking while you are still experimenting and making mistakes on the side.

The staging area is like a packing list. Using git add lets you choose exactly which files are ready to be saved into your next commit. This stops you from accidentally saving messy drafts or incomplete files into your final project history.
