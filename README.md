# Homework 00
These introductory tasks are intended to prepare for Matlab coding exercises. This includes set-up of a code reviewing and management system, and a basic introduction to computational methods to solve differential equations. 

1. Create a GitHub account if you do not already have one. GitHub will be the primary means of distributing assignments and submitting completed code and other exercises. It uses the Git source code management system, which is useful for version control, bug fixing, and issue tracking in many software projects. The following additional tasks are suggested.
    1.  Set up [Git software](https://git-scm.com/downloads) and [Matlab](https://www.mathworks.com) on the local machine that you will use for coding. For your code, also set up a local repository, which is a Git-aware directory. Much of the interaction with git will take place from a command-line terminal. However, it may also be helpful to use a Git [desktop app](https://desktop.github.com) to be able to track code changes visually.
    2. It is recommended to work through a Git tutorial. There are many excellent tutorials available, including sandboxed versions that run separate from your PC: [Introduction sequence](https://learngitbranching.js.org/) and a [visualized sandbox](http://git-school.github.io/visualizing-git/). Recent versions of Matlab are also integrated with Git, and there are some [Matlab-specific tutorials](https://admin.kuleuven.be/icts/onderzoek/wetsoft/software/matlab/pdf/versioning-git-matlab.pdf) and [blog postings](https://blogs.mathworks.com/community/2014/10/20/matlab-and-git/). Try to understand how to clone or checkout a repository, and commit changes.
    3. Email your GitHub username to the instructor. This will allow you to be invited to join the course's Classroom site.
  
 2. Familiarize yourself with Matlab's tools for solving ordinary differential equations. The [ballode.m](https://github.com/biomechanics-course/hw00/blob/master/ballode.m) demo shows how to simulate a ball bouncing on the ground. In particular, look up the `ode23` (or `ode45`) command documentation, and read about event detection.
     1. Starting with `ballode`, create a new simulation `ballodebounceandhalf` that has slightly different dynamics. Modify the flight dynamics to include viscous drag force `-B*v`, where `v` is ball velocity. (Treat the ball's mass as 1.) Also modify the coefficient of restitution for the bounce to equal -0.5.
     2. Instead of performing 10 flight segments, only simulate 2. And after the first bounce, terminate the simulation by detecting the apex of the ball's flight (zero velocity).

3.  Familiarize yourself with GitHub Markdown, which is a method for formatting text within a repository. Use Markdown to record answers to the following questions.

4.  Consider how to simulate a different second-order differential equation, the inverted pendulum, theta'' - wn\*theta = 0, where wn is the natural frequency (omega-n) equal to 1. Describe the modifications needed to convert the ballode demo into an inverted pendulum simulation. (No need to perform the simulation, just describe how it would be done, in a few sentences.)

5. Consider how to simulate a first-order differential equation, such as x-dot + 1x = 0, with initial condition x(0) = 1. Describe how the above ODE commands would have to be modified to solve this equation. (No need to perform the simulation.)

6. Contribute to the hw00 repository by either filing or responding to an Issue. Ask a question about anything related to the assignment, or answer the question, or participate in a discussion in any way. Alternatively, try improving this `README.md` file or the `ballode.m` code, and filing a pull request.
