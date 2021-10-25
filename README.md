echo "initial file" > K.txt
git add K.txt
git commit -m "Commit A"
git checkout -b foo master
echo "foo" > k.txt
git commit -a -m "Commit B"
git checkout -b bar master
echo "bar" > k.txt
git commit -a -m "Commit C"
git merge foo
echo "foobar" > k.txt
git commit -a -m "Commit M"
echo "2nd line" >> k.txt
