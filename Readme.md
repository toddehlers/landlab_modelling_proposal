# Development of a source-to-sink stratigraphic prediction framework
## (Dr. Nevena Andrić Tomašević)

## 1. Product description: techincal details
**Requirements.** The proposed source-to-sink stratigraphic prediction framework (**SSPF**) will use physical laws to simulate
geological processes operating in the source and sink areas to be able to predict anatomy of sedimentary basin.

**Software architecture.** The proposed SSPF will  be designed as a component based software with user-friendly interface.
Each component will represent self-contained peace of code that provide numerical representation of a single geological process.
There are several advantages of the software architecture like this. One of the main advantages is ability to re-use already
existing components instead of writing them from the scratch. Therefore, this approach can significantly reduce development
time and costs. Furthermore, such software architecture gives ability to re-use and integrate **in-house proprietary components
developed by the applicant or even whole framework into other systems.** For example the proposed SSPF can be integrated into
commercial softwares used in oil and gas industry Dyonisos, GMP, Petrel. 

The SSPF will be able to operate on the desktop computers. Also the simulations will be able to run using high performance
computing (HPC) facilities that are routinely used in numerous oil and gas companies. All coded components will be hidden behind
graphical user interface (GUI). Instead of using special terminology and memorizing commands the user will be able to add input
parameters in the fields on the GUI and easily startmodel run. Therefore, user does not need to know the details of the code.
Furthermore, the software documentation will include adequate default values to decrease need for sensitivity studies. 

## 2. Product development methodology
The SSPF will be created using a **Landlab toolkit and Phyton as a programming language**.  Landlab is a open-source Phyton based
toolkit designed for building, coupling and exploring numerical models of Earth-surface dynamics (Hobley et al., 2017).
There are several advantages of using Landlab toolkit. First advantage of Landlab is the existence of **infrastructure, and
re-usable libraries and components** written to solve specific Earth-surface processes. Second, Landlab components have written
following standardized prodecure that makes easier linkage and operability between components with only one or two lines of
code, and allowing **time-effective integration.** Therefore, the new components written by the applicant will be written in Phyton
following Landlab procedures. Third advantage of Landlab is an opportunity to use **best practice extensive and automated testing
processes** to test key functionalities of components, integration process and final product/framework. 

The main advantage of using a Phyton programming language is that besides giving me ability to work in Landlab toolkit allows
easier integration of **SSPF into GPM model** developed by my industrial colaborator Wintershall. 
Graphical user interface (GUI) will be created using the Rust programming language.

## 3. Work packages (WP) and division of labour
The overall structure of the project can be divided into 8? work packages that are detailed below. All of this work will be
conducted by applicant as a post-doctoral researcher at the University of Tübingen. In detail, the applicant Dr. Nevena Andrić
Tomasevic will coduct work neccesary for the work packages WP1, WP2, WP3, WP4 and WP7 in collaboration with prof. Dr. Todd Ehlers,
Willi Kappler and industrial partner, Wintershall.  The WP5 will be done by HIWI student from computer sciences (master level)
supervised by Willi Kappler with interaction with applicant. Data compilation in the WP7 will be obtained by student assistant
(geosciences, master level) under supervision of the applicant.  

**I am proficient in Phyton coding necesssary to complete WP1, WP2 and WP3. Furthermore, I have ~ 4 years of experience in various
geological processes numerical and running numerical models on high performance computing (HPC) facilities that is needed to
complete WP6.**

**My PhD experience on the interaction between tectonic and sedimentation gives me ability to judge necessary requirements for
development of new components, but also to select necessary re-usable components. Moreover, I am proficient in basin and mountain
range data analysis neccesary to complete WP6, as demonstrated by my previous publications.**

### WP1. Development of source area tectonic component
Staff: Post-doc – my own position (2 years)

The main objectives of this work package are creation of source area tectonic component and associated development document to be
used in the framework integration WP3. The main tasks are creation of source code that handles all parameters necessary to define
tectonic activity in the source area and development documentation. After unit testing in the WP4, this component will be used to
assemble the SSPF in WP3. 

### WP2. Re-usable component  customization
Staff: Post-doc – my own position (2 years)

This work package aims at modification of the selected re-usable components so they can be included in SSPF framework. The main
tasks are modification of the components for specific requirement, preformance of necassary changes so the component can run in the
framework and upgrading the specific component to get a better performance or higher quality. After unit testing in the WP4, these
components will be used to assemble the SSPF in WP3. 

### WP3. Framework integration
Staff: Post-doc – my own position (2 years)

This work package aims at assembling new and re-usable components (results of WP1 and WP2) into final framework. The main tasks are
providing communication and coordination between components. This will be done by creation of peaces of code. The output of this work
package is final SSPF ready to be subjected to system testing phase, WP4. Additional output
is framework integration documentation necessary for further system maintenance and service, WP8. 

### WP4. Testing
Staff: Post-doc – my own position (2 years)

Objectives of this work package are to confirm that components (results of WP1 and WP2) and framework (result of WP 3) satisfy the
requirements, and indentify and correct defects in the framework implementation. Tasks of this work package are functionality and
riability testing of 1) unit/component, 2) process of component integration, and 3) finally assembled framework. This will be done
using standard and certified testing procedures in the frame of Landlab toolkit. Testing documentation for system maintenance will
be output of this work package. 

### WP5. Creation of user-friendly interface
Staff: Student assistant („HIWI“, 2 years)

Objective of WP5 is design and creation of user-friendly interface. Tasks will be:
- Set up / configure Apache web server
- Develop server side web application in Rust
- Design client side web based GUI with HTML5, CSS and JavaScript
- Integration testing of SSPF and web GUI

### WP6. Evaluation of the framework
Staff: Student assistant („HIWI“, 1 year),
Staff: Post-doc – my own position (2 years)

This work package aims at evaluating final product (SSPF) using real geological data. The main tasks are 1) compilation of real
geological data from the case study area, and 2) running a numerical models using framework on high performance computing facilities.

**Case study will be Molasse Basin and surrounding Alpine mountain range. The geological data consernig Molasse basin will be provided
by the industry partner Wintershall. Necessary data on Alpine mountain range will be collected from the existing literature. Moreover,
the Earth System Dynamics Group at the University of Tuebingen has in-depth experience in research of the tectonic and erosional
processes in the Alpine mountain range.**

### WP7.  Communication and dissemination of the source-to-sink stratigraphic prediciton framework
Staff: Post-doc – my own position (2 years)

This work package aims at promotion of project objectives, developments and results to all potential users and interested partners at
local, national and European/world level. Tasks will include communicating project objectives, developments and results on the conferences,
showcases and through peer-review and technical publications. 

### WP8.  System maintenance and service???
Staff: Post-doc – my own position (after project completion)

## 4. Equipment available in the Earth System Dynamics Working Group, University of Tübingen
**Linux cluster:** for this project I will have unrestricted access to the linux cluster in Prof. Ehlers work group (see Ehlers` support
letter). This cluster includes 360 cores, 12 GB RAM per core, and 290 TB storage capacity for high performance computing for the testing
and evaluation of source-to-sink stratigraphic prediciton framework; programs needed (Paraview, Arc-Gis, Phyton) are installed and
routinely used in the Earth System Dynamics Working Group. 
