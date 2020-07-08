# bugzilla quips fortunes

My fortune file from bugzilla quips

- Install fortune-mod
~~~
sudo dnf install fortune-mod
~~~

- Copy the bugzilla quips from the files `onliner` and `oneliner.dat`

~~~
sudo cp oneliner oneliner.dat /usr/share/games/fortune/
~~~

- Add to `~/.bashrc`
~~~
echo  -e "\033[33;7m$(fortune)\033[0m"
~~~

You can create your own fortunes by adding `%` between quotes and generate the dat file `strfile -c % oneliner.txt oneliner.dat`

If you do not care for online database or just want it from one file you can use 
~~~
echo  -e "\033[33;7m$(shuf -n 1 ~/quips/oneliner.txt)\033[0m"
~~~

My final ~/.bashrc 
~~~
echo  -e "\033[33;7m$( fortune 60% oneliner hitchhiker 20% kernelnewbies osfortune )\033[0m"
~~~
