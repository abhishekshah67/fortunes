# bugzilla quips fortunes

My fortune file from bugzilla quips

- Install fortune-mod
~~~
sudo dnf install fortune-mod
~~~

- Copy the bugzilla quips from the files `onliner.txt` and oneliner.dat

~~~
cp oneliner.* /usr/share/games/fortunes/
~~~

You can create your own fortunes by adding `%` between quotes and generate the dat file `strfile -c % oneliner.txt oneliner.dat`
