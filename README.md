# 计算机图形学初级课程

This is a computer graphics course for entry-level learner. Course designed by [Assistant Prof. Chenlei Lv](https://aliexken.github.io/),
Shenzhen University, with assistance from VCCLab and CSSE.

## 前言

本课程面向计算机图形学初学者，以帮助他们尽快了解图形学渲染管线，几何变换，图形接口编程等基础知识。学习该课程最好需要具备C++编程、数据结构、线性代数等前置知识，这会大大提升学习效率。当然，我会尽可能在课程中增加相关概念的解释。

针对计算机图形学教学，大部分教材与课程设置，默认以OpenGL作为学习对象，以完成对图形学内容的解释和实践。遵从传统，我们使用OpenGL3.0+作为图形编程接口，

In general, the materials in this course assume that students should have
already taken **Linear Algebra** and **Calculus**.

Students should have already taken **Introduction to Computer Science** and should
be proficient in computer programming (in any language) and should feel
comfortable programming in **C++**. 

_All course assignments are conducted in C++, however none rely on nitty gritty
memory management or complicated object-oriented data-structures._

While knowledge of **Partial Differential Equations** _is not required_, it will
certainly be very handy for derivations. Similarly, previous experience with
**Computer Graphics** _is not required_ but recommended.

All coding assignments make use of
[Eigen](https://en.wikipedia.org/wiki/Eigen_(C%2B%2B_library)), an open-source
linear algebra library; and [libigl](http://libigl.github.io/libigl/), an
open-source geometry processing library.  Each assigment is built using
[CMake](https://en.wikipedia.org/wiki/CMake).


## Organization

The [original run](http://www.cs.toronto.edu/~jacobson/geometry-processing/) of
this course structured _weekly_ assignments in the following order:

 1. [Introduction](https://github.com/alecjacobson/geometry-processing-introduction)
 2. [Mesh Reconstruction](https://github.com/alecjacobson/geometry-processing-mesh-reconstruction) 
 3. [Surface Registration](https://github.com/alecjacobson/geometry-processing-registration) 
 4. [Smoothing](https://github.com/alecjacobson/geometry-processing-smoothing) 
 5. [Parameterization](https://github.com/alecjacobson/geometry-processing-parameterization)
 6. [Deformation](https://github.com/alecjacobson/geometry-processing-deformation) 
 7. [Curvature](https://github.com/alecjacobson/geometry-processing-curvature)

Besides the introduction, there is no strict ordering to these topics.

Each topic has its own git repository. Inside each, there is a `README.md` file
contains background information necessary for understanding the topic's coding
assignment. 

The
[Introduction](https://github.com/alecjacobson/geometry-processing-introduction)
`README.md` contains detailed information about compilation, file layout and
assignment protocols. 

## Wikipedia

The background materials link heavily to Wikipedia articles. Sometimes the
wikipedia articles relating to geomtry processing are less informative than they
could be. Edit them!

In university offerings of this course, 5% credit has been awarded to the entire
class for collaboratively improving Wikipedia's entries on geometry processing
topics. 

## Are you an instructor?

There are instructor repositories for all of the assignments above. If you're an
instructor for a geometry processing course, send an email to
jacobson@cs.toronto.edu for an invitation.

> For my reference, I can add a new instructor with github id [githubid] to all solution repos using:
>
>     github-add-user -u alecjacobson -r $(echo alecjacobson/geometry-processing-{introduction,mesh-reconstruction,registration,smoothing,parameterization,deformation,curvature}-solution | tr ' ' ',') [githubid]

### Corresponding solution (private) repos are located at:

 1. [Introduction](https://github.com/alecjacobson/geometry-processing-introduction-solution)
 2. [Mesh Reconstruction](https://github.com/alecjacobson/geometry-processing-mesh-reconstruction-solution) 
 3. [Surface Registration](https://github.com/alecjacobson/geometry-processing-registration-solution) 
 4. [Smoothing](https://github.com/alecjacobson/geometry-processing-smoothing-solution) 
 5. [Parameterization](https://github.com/alecjacobson/geometry-processing-parameterization-solution)
 6. [Deformation](https://github.com/alecjacobson/geometry-processing-deformation-solution) 
 7. [Curvature](https://github.com/alecjacobson/geometry-processing-curvature-solution)

### Homework Submission via GitHub Pull Requests

When used for a formal course, it is intended that students _fork_ each
assignments repository, _commit_ their solutions to their own forks, and then
submit their assignment via _pull request_ to the public repo of the assignment.

More details on this structure are found on [Alec's
weblog](http://www.alecjacobson.com/weblog/?p=4700).

#### Honor System

Since pull requests are public, students will be able to see each other's
completed solutions as soon as their posted. _Students will not cheat because
they are honorable 👍._ Actually, since most of the assignments are standard
algorithms there are _many_ implmentations online already. In particular, libigl
contains ready-made implementations using Eigen with similar function APIs. Why
cheat from other students when you can cheat from the professor? But, really,
why cheat?
