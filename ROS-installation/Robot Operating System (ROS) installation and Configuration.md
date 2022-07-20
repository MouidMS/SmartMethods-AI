<h1>Robot Operating System (ROS) installation and Configuration</h1>
  <h3>Steps:</h3>
    <ul>
      <li>Install VMware.</li>
  <li>Download Ubunto 16.4.</li>
  <li>Setup.</li>
  <li>Install ROS kinetic And Run.</li>
    </ul>
    <h3>1-Install VMware</h3>
    https://www.vmware.com/go/getworkstation-win
    <img src='https://user-images.githubusercontent.com/75043063/179870848-ab49910c-4e7b-401c-b247-f7a3ed0d2441.png'><img/>
    <h3>2-Download Ubunto 16.4</h3>
    https://releases.ubuntu.com/16.04/
    
   
   <h3>3-Setup</h3>
<img src='https://user-images.githubusercontent.com/75043063/179871108-87a063f9-3048-43e1-87e6-1566710ca68a.png'/>
   <h3>Install ROS kinetic And Run</h3>
   Setup your sources.list:
   <pre>sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
</pre>

<h3 dir="auto"><a id="user-content-setup-your-sourceslist" class="anchor" aria-hidden="true" href="#setup-your-sourceslist"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Setup your sources.list</h3>
<div class="highlight highlight-text-shell-session notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="sudo sh -c 'echo &quot;deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main&quot; &gt; /etc/apt/sources.list.d/ros-latest.list'
"><pre><span class="pl-c1">sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" &gt; /etc/apt/sources.list.d/ros-latest.list'</span>
</pre></div>
<h3 dir="auto"><a id="user-content-set-up-your-keys" class="anchor" aria-hidden="true" href="#set-up-your-keys"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Set up your keys</h3>
<div class="highlight highlight-text-shell-session notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="sudo apt install curl "><pre><span class="pl-c1">sudo apt install curl </span></pre></div>
<div class="highlight highlight-text-shell-session notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
"><pre><span class="pl-c1">curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -</span>
</pre></div>
<h3 dir="auto"><a id="user-content-installation-1" class="anchor" aria-hidden="true" href="#installation-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Installation</h3>
<div class="highlight highlight-text-shell-session notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="sudo apt-get update"><pre><span class="pl-c1">sudo apt-get update</span></pre></div>
<p dir="auto">Desktop-Full Install: (Recommended) </p>
<div class="highlight highlight-text-shell-session notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="sudo apt-get install ros-kinetic-desktop-full
"><pre><span class="pl-c1">sudo apt-get install ros-kinetic-desktop-full</span>
</pre></div>
<p dir="auto">To find available packages, use:</p>
<div class="highlight highlight-text-shell-session notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="apt-cache search ros-kinetic">
    <pre>apt-cache search ros-kinetic</pre>
<h3 dir="auto"><a id="user-content-environment-setup" class="anchor" aria-hidden="true" href="#environment-setup"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Environment setup</h3>
<div class="highlight highlight-text-shell-session notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="echo &quot;source /opt/ros/kinetic/setup.bash&quot; &gt;&gt; ~/.bashrc
"><pre><span class="pl-c1">echo "source /opt/ros/kinetic/setup.bash" &gt;&gt; ~/.bashrc</span>
</pre></div>
<div class="highlight highlight-text-shell-session notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="source ~/.bashrc
"><pre><span class="pl-c1">source ~/.bashrc</span>
</pre></div>
<div class="highlight highlight-text-shell-session notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="source /opt/ros/kinetic/setup.bash
"><pre><span class="pl-c1">source /opt/ros/kinetic/setup.bash</span>
</pre></div>
<p dir="auto">If you use zsh instead of bash you need to run the following commands to set up your shell:</p>
<div class="highlight highlight-text-shell-session notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="echo &quot;source /opt/ros/kinetic/setup.zsh&quot; &gt;&gt; ~/.zshrc
source ~/.zshrc"><pre><span class="pl-c1">echo "source /opt/ros/kinetic/setup.zsh" &gt;&gt; ~/.zshrc</span>
<span class="pl-c1">source ~/.zshrc</span></pre></div>
<h3 dir="auto"><a id="user-content-dependencies-for-building-packages" class="anchor" aria-hidden="true" href="#dependencies-for-building-packages"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Dependencies for building packages</h3>
<p dir="auto">To install this tool and other dependencies for building ROS packages, run:</p>
<div class="highlight highlight-text-shell-session notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential"><pre><span class="pl-c1">sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential</span></pre></div>
<h4 dir="auto"><a id="user-content-initialize-rosdep" class="anchor" aria-hidden="true" href="#initialize-rosdep"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Initialize rosdep</h4>
<div class="highlight highlight-text-shell-session notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="sudo apt install python-rosdep
"><pre><span class="pl-c1">sudo apt install python-rosdep</span>
</pre></div>
<p dir="auto">With the following, you can initialize rosdep.</p>
<div class="highlight highlight-text-shell-session notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="sudo rosdep init
rosdep update"><pre><span class="pl-c1">sudo rosdep init</span>
<span class="pl-c1">rosdep update</span></pre></div>
<h3 dir="auto"><a id="user-content-build-farm-status" class="anchor" aria-hidden="true" href="#build-farm-status"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Build farm status</h3>
<p dir="auto">Create the catkin root and source folders:</p>
<pre>sudo apt-get install ros-kinetic-catkin
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/</pre>
    
<p dir="auto">Configure the catkin workspace by issuing a first “empty” build command:</p>
<div class="highlight highlight-text-shell-session notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="catkin_make
cd ~/catkin_ws/src
"><pre><span class="pl-c1">catkin_make</span>
<span class="pl-c1">cd ~/catkin_ws/src</span>
</pre></div>
<h2 dir="auto"><a id="user-content--lunch-ros" class="anchor" aria-hidden="true" href="#-lunch-ros"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><ins> Lunch ROS.</ins></h2>
<p dir="auto">Launching ROS on a project robotic arm , Clone Github repository.</p>
<div class="highlight highlight-text-shell-session notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="git clone https://github.com/smart-methods/arduino_robot_arm.git "><pre><span class="pl-c1">git clone https://github.com/smart-methods/arduino_robot_arm.git </span></pre></div>
<p dir="auto">Check the dependencies:</p>

<pre>
cd ~/catkin_ws

rosdep install --from-paths src --ignore-src -r -y</pre>

<pre>
sudo apt-get install ros-kinetic-moveit

sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui

sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher

sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control</pre>

<p dir="auto">The final command to finally launch the project</p>
    <pre><span class="pl-c1">roslaunch robot_arm_pkg check_motors.launch</span>
</pre></div>
<img src='https://user-images.githubusercontent.com/75043063/179872937-419c4583-60b8-4e8f-9679-a38f8693ec82.png' >
   
