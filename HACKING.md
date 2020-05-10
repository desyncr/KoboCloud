# Mounting kobo

mkdir -p /media/kobo
sudo mount -t vfat /dev/sdb /media/kobo -o rw,uid=1000,gid=1000

# Unmounting

sudo umount /media/kobo

# Copy

sh ./makeKoboRoot.sh
cp KoboRoot.tgz /media/kobo/.kobo
