# Install java on linux

# Description 💬

How to install java and javac on linux any version via easy step

# Disclaimer ⚠️

We will install “jdk-19” .
In the future if you install jdk-20 your command will stand for “jdk-20” instead , Are you understand?

# Dependency ✋

Download site of java officials : 

[Download the Latest Java LTS Free](https://www.oracle.com/java/technologies/downloads/)

# Download & Install 🛠️

1. Download with file .deb (x64 Debian Package)

![Untitled](Install%20java%20on%20linux%2049ceb8d991384aaa943406177a4c00cd/Untitled.png)

1. Go to download directory

![Untitled](Install%20java%20on%20linux%2049ceb8d991384aaa943406177a4c00cd/Untitled%201.png)

1. Select file and open with “Software Install”

![Untitled](Install%20java%20on%20linux%2049ceb8d991384aaa943406177a4c00cd/Untitled%202.png)

1. Click to Install via this program

![Untitled](Install%20java%20on%20linux%2049ceb8d991384aaa943406177a4c00cd/Untitled%203.png)

1. Go to terminal

![Untitled](Install%20java%20on%20linux%2049ceb8d991384aaa943406177a4c00cd/Untitled%204.png)

1. Tell terminal where package we are install

```bash
sudo update-alternatives --install "/usr/bin/java" "java" "/usr/lib/jvm/jdk-19/bin/java" 1
```

![Untitled](Install%20java%20on%20linux%2049ceb8d991384aaa943406177a4c00cd/Untitled%205.png)

1. Set path

```bash
sudo update-alternatives --set java /usr/lib/jvm/jdk-19/bin/java
```

![Untitled](Install%20java%20on%20linux%2049ceb8d991384aaa943406177a4c00cd/Untitled%206.png)

1. Verify what’s version we use

```bash
sudo update-alternatives --config java
```

![Untitled](Install%20java%20on%20linux%2049ceb8d991384aaa943406177a4c00cd/Untitled%207.png)

check your terminal know your java with 

```bash
java --version
```

![Untitled](Install%20java%20on%20linux%2049ceb8d991384aaa943406177a4c00cd/Untitled%208.png)

<aside>
💡 We will do step 6 to step 8 again for setting javac path

</aside>

1. For javac we will do again with this below command

```bash
# step 6 : tell terminal where are javac install
sudo update-alternatives --install "/usr/bin/javac" "javac" "/usr/lib/jvm/jdk-19/bin/javac" 1

# step 7 : set path 
sudo update-alternatives --set javac /usr/lib/jvm/jdk-19/bin/javac

# step 8 : check version we use
sudo update-alternatives --config javac

# check version :
javac --version
```

To this you will complete set javac and java on linux!

# Tips 🧐

After we install Step 4 my java package will store on path

```bash
/usr/lib/jvm/jdk-19
```

![Untitled](Install%20java%20on%20linux%2049ceb8d991384aaa943406177a4c00cd/Untitled%209.png)

if we go to this path we will see the bin directory

![Untitled](Install%20java%20on%20linux%2049ceb8d991384aaa943406177a4c00cd/Untitled%2010.png)

And lastly you will see javac and java on this path.
Then we will set path on this OKAY!?

```bash
java => /usr/lib/jvm/jdk-19/bin/java
javac => /usr/lib/jvm/jdk-19/bin/javac
```

![Untitled](Install%20java%20on%20linux%2049ceb8d991384aaa943406177a4c00cd/Untitled%2011.png)

# Author ✍️

[zergreen - Overview](https://github.com/zergreen)