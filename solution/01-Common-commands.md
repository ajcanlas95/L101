# 01 Common commands

This would be the solution of this exercise [here](https://github.com/ajohnsc/L101/blob/master/exercise/01-Common-commands.md)

If you need to review please click [here](https://github.com/ajohnsc/L101/blob/master/activities/01-Common-commands.md)

---

### Soluton

1. First start the activity with the workshop
```$ workshop basic launch
Creating example files.........Success
Creating example directories...Success
```
2. Create a file named `linux` inside `/home/student/dir1` directory

`$ touch /home/student/dir1/linux`

3. Remove the `/home/student/dir2` directory

`$ rmdir /home/student/dir2`

4. Create 3 files named `activityA`,`activityJ`,`activityC` in `/home/student/dir3` directory

`$ touch /home/student/dir3/activityA /home/student/dir3/activityJ /home/student/dir3/activityC`

5. Remove `/home/student/file1` and `/home/student/file3` file.

`$ rm /home/student/file1 /home/student/file3`

6. Redirect the output of `/etc/hostname` in `/home/student/file2`.

`$ cat /etc/hostname > /home/student/file2`

7. Print `"I am a Linux lover"` and append it to `/home/student/file2`.

`$ echo "I am a Linux lover" >> /home/student/file2`

8. Get which user you are using and redirect the output to a file named `/home/student/user`

`$ whoami > /home/student/user`

9. Get the content of `/var` then redirect the output in a file named `/home/student/variable`

`$ ls /var > /home/student/variable`

10. Get your current working directory then redirect in a file named `/home/student/directoryfile`

`$ pwd > /home/student/directoryfile`

11. Rate your work

`$ workshop basic rate`

12. If you get a passing overall score cleanup the environment for next lessons

`$ workshop basic clean`
