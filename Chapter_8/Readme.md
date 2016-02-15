#Chapter 8: Moving Around (pushd, popd)

##Do More

###Use these commands to move around directories all over your computer.

Commands used 
`cd temp`
`mkdir -p i/like/icecream`
`pushd i/like/icecream`
~/temp/i/like/icecream ~/temp
`popd`
~/temp
`pwd`
~/temp
`pushd i/like`
~/temp/i/like ~/temp
`pwd`
~/temp/i/like
`pushd icecream`
~/temp/i/like/icecream ~/temp/i/like ~/temp
`pwd`
~/temp/i/like/icecream
`popd`
~/temp/i/like ~/temp
`pwd`
~/temp/i/like
`popd`
~/temp
`pushd i/like/icecream`
~/temp/i/like/icecream ~/temp
`pushd`
~/temp ~/temp/i/like/icecream
`pwd`
~/temp
`pushd`
~/temp/i/like/icecream ~/temp
`pwd`
~/temp/i/like/icecream


###Remove the i/like/icecream directories and make your own, then move around in them.

##Explanation

The command's `pushd` and `popd` work like a scroll wheel through favorited directories.
When you `pushd` to a specific directory, you essentially bookmark yourself there. When you continue on through the path and `popd`, you will be taken back to your closest `pushd` directory.
This could be handy if you need to easily navigate through a very long path.
