---
permalink: /academics/
author_profile: true
redirect_from: 
---

{% include base_path %}

<div>
	<h1><p>Key Projects</p></h1>
	<hr style='background-color:#000000;border-width:0;color:#000000;height:2px;line-height:0;text-align:left;width:100%;'/>

		<h2><p>Image-to-Image Translation</p></h2>
	    <ul>
	        <li>Implemented CycleGAN in tensorflow for an image to image translation with a U-Net based architecture with additional residual layers as a generator, and a PatchGAN discriminator to generate Monet-esque style</li>
	    	<li>Trained the model using a custom TPU strategy with MSE loss along with gradient penalty for the discriminator, while the generator is optimized with the Adversarial Loss, Cyclic Consistency Loss and Identity Loss</li>
	    </ul>

	    <h2><p>Wasserstein GAN</p></h2>
	    <ul>
	        <li>Trained a Convolutional Generative Adversarial Network on the simple MNIST dataset to generate hand-written images of digits with improved stability by implementing Gradient Penalty on Wasserstein Loss for the critic to avoid modal collapses</li>
	    	<li>Updated the critic multiple times for every update to the generator to prevent the generator from overpowering the critic</li>
	    </ul>

	    <h2><p>Automatic Image Colorization</p></h2>
	    <ul>
	        <li>Trained a Deep Neural Network with CNNs and Inception-ResNet-v2 using the luminate component of an image by first extracting the mid and high-level features from the encoder and inceptionnet (trained on ImageNet dataset) and merging them before passing to the decoder to estimate the ab components as described in Baldassarre et.al's Deep Koalarization paper</li>
    	    <li>Colored the image using this model by converting the predicted ab channels combined with input l channel to RGB space</li>
	    </ul>

	    <h2><p>Neural Style Transfer</p></h2>
	    <ul>
	        <li>Implemented a Neural Style Transfer Algorithm to generate artificial images by manipulating the content image using the appearance or visual style of the style image as described in Gatys et al</li>
    	    <li>Minimized cost with the content image (as the distance between activations) and the style image (as the distance between the gram matrices) on multiple layers using a pre-trained VGG-19 CNN on ImageNet dataset</li>
	    </ul>

		<h2><p>Image Segmentation</p></h2>
	    <ul>
	        <li>Implemented the U-Net architecture of the encoder, decoder blocks with convolutional layers in tensorflow and trained on the CARLA self-driving car dataset with sparse categorical crossentropy for pixelwise prediction</li>
	    </ul>

	    <h2><p>Real Time Face Mask Detection</p></h2>
	    <ul>
	        <li>Trained a CNN model using sample data from a Kaggle dataset with Convolution and Max Pooling layers to extract features, and finally classify using dense layers with softmax activation function with an accuracy of 97\%</li>
    		<li>Classified images by detecting faces using Haar Cascade Frontal Face classifier and predict whether mask is present or not</li>
	    </ul>

	    <h2><p>Image Matching</p></h2>
	    <ul>
	        <li>Used Scale Invariant Feature Transform (SIFT) technique to generate keypoints that are scale-invariant and rotation invariant and used these as features to match images in OpenCV</li>
	    </ul>

	    <h2><p>Invisibility Cloak</p></h2>
	    <ul>
	        <li>Developed an invisibility cloak application using simple vision techniques in OpenCV</li>
    	    <li>Transformed the image from RGB space to Hue-Saturation-Value (HSV) space accounting for different shades and intensities of a specific shades to detect the red color cloth, and replaced the segmented red cloth with initial background</li>
	    </ul>

	    <h2><p>Keyframe Animation</p></h2>
	    <p><i>Guide : <a href="https://www.cse.iitb.ac.in/~paragc/">Prof. Parag Chaudhuri</a>, IIT Bombay</i></p>
	    <ul>
	        <li>Designed an interactive modeling tool in C++ OpenGL to create 3D models from triangle meshes</li>
    		<li>Implemented modeling-viewing pipeline to convert the scene from 3D perspective to 2D planar view along with clipping</li>
    		<li>Created 3D models using hierarchical modeling from scratch and animated them using Keyframe Interpolation</li>
	    </ul>

	    <h2><p>Regret Minimisation Algorithms</p></h2>
	    <p><i>Guide : <a href="https://www.cse.iitb.ac.in/~shivaram/">Prof. Shivaram Kalyanakrishnan</a>, IIT Bombay</i></p>
	    <ul>
	        <li>Implemented various Upper Confidence Bound (UCB) algorithms namely UCB, $\beta$-UCB, Adaptive $\beta$-UCB, UCB-tuned for a Stochastic Multi Arm Bandit setting to analyze the regret and cumulative regret and compare performance of algorithms which take empirical variance of arms also into account to those which only consider mean</li>
	    </ul>

		<h2><p>Similar Language Detection</p></h2>
	    <p><i>Guide : <a href="https://www.cse.iitb.ac.in/~ganesh/">Prof. Ganesh Ramkrishnan</a>, IIT Bombay</i></p>
	    <ul>
	        <li>Followed a hierarchial way by dividing languages into groups using cosine similarity for feature vector with frequencies of words in training set</li>
	        <li>Trained different Support Vector Machines (SVM) for each language group with features engineered from character n-grams and word n-grams</li>
	        <li>Used tf-idf-qf scoring for assigning weights to elements in feature vector and used ensemble methods with mean confidence to combine the different classifiers</li>
	    </ul>

	    <h2><p>Optical Character Recognition & The Pac-Man Projects</p></h2>
	    <p><i>Guide : <a href="https://www.cse.iitb.ac.in/~shivaram/">Prof. Shivaram Kalyanakrishnan</a>, IIT Bombay</i></p>
	    <ul>
	        <li>Implemented various classifiers like Perceptron, MIRA, neural networks for  extracting text from scanned handwritten images</li>
    	    <li>Implemented various search algorithms for pacman agent to find paths namely DFS, BFS, Uniform Cost Search, A* Search, Minimax Search, Expectimax Search</li>
    		<li>Implemented particle filter algorithm that tracks individual and multiple ghost agents simultaneously in Dynamic Bayes Net</li>
	    </ul>

	    <h2><p>Compiler for C-like Language</p></h2>
        <p><i>Guide : <a href="https://www.cse.iitb.ac.in/~uday/">Prof. Uday Khedkher</a>, IIT Bombay</i></p>
        <ul>
            <li>Developed a compiler for fundamental C constructs along with live variable analysis for dead code elimination</li>
            <li>Incorporated features like lexical analysis, parsing, symbol table creation, intermediate code generation and assembly level code generation using FlexC++ and BisonC++</li>
        </ul>

        <h2><p>Project Database Management</p></h2>
        <p><i>Guide : <a href="https://www.cse.iitb.ac.in/~sudarsha/">Prof. S. Sudarshan</a>, IIT Bombay</i></p>
        <ul>
            <li>Built a java based web portal that assists in searching and applying for projects in certain area of interest using servlets, PostgreSql, Ajax in JavaScript queries</li>
            <li>Implemented professor and student portals where in professor can add new projects along with descriptions and accept the requests from students, student can review the projects based on his experience with the professor</li>
        </ul>

        <h2><p>SAT Solver</p></h2>
        <p><i>Guide : <a href="https://www.cse.iitb.ac.in/~supratik/">Prof. Supratik Chakraborthy</a> and Prof. Ashwin Gumaste, IIT Bombay</i></p>
        <ul>
            <li>Developed a VHDL based module for checking the satisfiability of 64 bit clauses</li>
            <li>Implemented Davis–Putnam–Logemann–Loveland (DPLL) algorithm along with Maximum Occurrences in clauses of Minimum Size (MOM's) Heuristic for checking the satisfiability of a formula</li>
        </ul>

        <h2><p>Distributed Password Cracker</p></h2>
        <p><i>Guide: <a href="https://www.cse.iitb.ac.in/~chebrolu/">Prof. Kameswari Chebrolu</a>, IIT Bombay</i></p>
        <ul>
            <li>Created a module that cracks password using the processing power of multiple machines working simultaneously using Socket Programming in C++</li>
            <li>Handled multiple client requests across different machines to a single server with multiple worker machines reliably using TCP while maintaining fairness by preventing clients from hogging resources</li>
        </ul>

        <h2><p>Branch Change Allocation</p></h2>
        <p><i>Guide : <a href="https://www.cse.iitb.ac.in/~sharat/">Prof. Sharat Chandran</a>, IIT Bombay</i></p>
        <ul>
            <li>Implemented modified Gale Shapley algorithm for college admissions in Python</li>
            <li>Constraints like limits on branch-strength and reservations simultaneously maintaining fairness were handled efficiently</li>
            <li>Developed a Django based web application that incuded a portal for users to fill their institute preferences</li>
        </ul>

        <h2><p>PinBall Simulation</p></h2>
        <p><i>Guide : <a href="https://www.cse.iitb.ac.in/~sharat/">Prof. Sharat Chandran</a>, IIT Bombay</i></p>
        <ul>
            <li>Designed a Rube Goldberg Machine that served the purpose for the simulation of the game by using multiple physics situations like spring forces, collisions</li>
            <li>Programmed in Box2D, a physics simulation engine using C++ platform</li>
            <li>Generated the same in a compiler independent way using cmake, a cross platform make system</li>
        </ul>

        <h2><p>Tic-Tac-Toe & Quantum-Tic-Tac-Toe</p></h2>
        <p><i>Guide : <a href="https://www.cse.iitb.ac.in/~supratik/">Prof. Supratik Chakraborthy</a> and <a href="https://www.cse.iitb.ac.in/~dbp/">Prof. Deepak B Phatak</a>, IIT Bombay</i></p>
        <ul>
            <li>Designed the popular game using Simple Cpp library by Prof. Abhiram Ranade (A C++ version by IIT-Bombay)</li>
            <li>Implemented multiplayer mode in Tic-Tac-Toe, Quantum-Tic-Tac-Toe and also implemented one player mode in Tic-Tac-Toe with different difficulty levels</li>
            <li>Used an algorithm which recursively backtracks to check the collapse of an entity in the game</li>
        </ul>
	<br>

	<h1><p>Technical Proficiency</p></h1>
	<hr style='background-color:#000000;border-width:0;color:#000000;height:2px;line-height:0;text-align:left;width:100%;'/>
	<ul>
        <li><b>Proficient: </b>Python, TensorFlow, Keras, PyTorch, C/C++, Java, Slang, Bash, SQL, MS Excel</li>
        <li><b>Reasonably Experienced: </b>OpenCV, OpenGL, MATLAB, Octave, \LaTeX, JavaScript, React</li>
    </ul>
	<br>

	<h1><p>Achievements</p></h1>
	<hr style='background-color:#000000;border-width:0;color:#000000;height:2px;line-height:0;text-align:left;width:100%;'/>
	<ul>
		<li>All India Rank 18 in <a href="https://en.wikipedia.org/wiki/Joint_Entrance_Examination#JEE_Advanced" target="_blank">JEE Advanced</a> among 150,000 candidates<span style="float: right">2014</span></li>
        <li>Awarded AP grade* for outstanding performance in Principles of Data and System Security, Engineering Drawing and Geodesy courses<span style="float: right">2014-18</span></li>
	    <li>100 percentile in <a href="https://en.wikipedia.org/wiki/Joint_Entrance_Examination#JEE_Main" target="_blank">JEE Mains</a> in B.Tech and 99.98 percentile in B.Arch among 1.4 million candidates<span style="float: right">2014</span></li>
	    <li>State Rank 2 in Andhra Pradesh <a href="https://en.wikipedia.org/wiki/Engineering_Agricultural_and_Medical_Common_Entrance_Test#Examination" target="_blank">EAMCET</a>, among 400,000 candidates<span style="float: right">2014</span></li>
		<li>All India Rank 64 in <a href="https://en.wikipedia.org/wiki/VIT_University" target="_blank"> VITEEE</a> out of 190,000 candidates<span style="float: right">2014</span></li>
		<li>Scored 422/450 in <a href="https://en.wikipedia.org/wiki/Birla_Institute_of_Technology_and_Science" target="_blank">BITSAT</a> Examination held by Birla Institute of Technology<span style="float: right">2014</span></li>
		<li>Among the top 300 in Indian National Astronomy Olympiad (<a href="https://en.wikipedia.org/wiki/National_Standard_Examination_in_Astronomy" target="_blank">INAO</a>)<span style="float: right">2014</span></li>
		<li>Awarded certificate of merit for top 1% in National Standard Examination in Physics (<a href="https://en.wikipedia.org/wiki/Indian_National_Physics_Olympiad" target="_blank">NSEP</a>)<span style="float: right">2014</span></li>
		<li>Attended Vigyan Jyoti Shivir (<a href="http://kvpy.iisc.ac.in/main/index.htm" target="_blank">Vijyoshi Camp</a>) at Indian Institute of Science, Bangalore (IISc)<span style="float: right">2013</span></li>
		<li>Among the top 35 and qualified to India finals in Indian National Junior Science Olympiad (<a href="https://olympiads.hbcse.tifr.res.in/about-olympiads/stages/science-olympiad/" target="_blank">INJSO</a>)<span style="float: right">2012</span></li>
		<li>State Rank 3 in Maths Olympiad by Andhra Prasedh Association of Mathematical Teachers (APAMT)<span style="float: right">2011</span></li>
    </ul>
    <p>*An AP grade is given to at most 1% of total students in a batch for excellent performance in the course</p>
	<br>

	<h1><p>Specializations & Courses on Coursera</p></h1>
	<hr style='background-color:#000000;border-width:0;color:#000000;height:2px;line-height:0;text-align:left;width:100%;'/>
		<div style="float: left; width: 50%;">
	        <ul>
	        	<li><a href="https://www.coursera.org/specializations/firstprinciplesofcomputervision" target="_blank">First Principles of Computer Vision Specialization</a></li>
	            <li><a href="https://www.coursera.org/specializations/deep-learning" target="_blank">Deep Learning Specialization</a></li>
	            <li><a href="https://www.coursera.org/specializations/generative-adversarial-networks-gans" target="_blank">Generative Adversarial Networks (GANs) Specialization</a></li>
	            <li><a href="https://www.coursera.org/specializations/tensorflow-advanced-techniques" target="_blank">TensorFlow: Advanced Techniques Specialization</a></li>
	            <li><a href="https://www.coursera.org/learn/machine-learning" target="_blank">Machine Learning</a></li>
	        </ul>
	    </div>

	    <div style="float: right; width: 50%;">
	        <ul style="list-style: none;">
	        	<li><a href="http://www.cs.columbia.edu/~nayar/" target="_blank">Prof. Shree K. Nayar</a></li>
	        	<li><a href="https://www.andrewng.org/" target="_blank">Prof. Andrew Ng</a></li>
	        	<li><a href="https://sharonzhou.me/" target="_blank">Prof. Sharon Zhou</a></li>
	        	<li><a href="https://laurencemoroney.com/" target="_blank">Prof. Laurence Moroney</a></li>
	        	<li><a href="https://www.andrewng.org/" target="_blank">Prof. Andrew Ng</a></li>
	        </ul>
	    </div>
	<br>

	<h1><p>Courses at IIT Bombay</p></h1>
	<hr style='background-color:#000000;border-width:0;color:#000000;height:2px;line-height:0;text-align:left;width:100%;'/>
		<div>
			<div style="float: left; width: 100%;"><h3><p>Spring 2017-18</p></h3></div>
	        <div style="float: left; width: 50%;">
	            <ul>
	            	<li>Biomedical Microsystems</li>
	                <li>Geodesy</li>
	                <li>Human Cognitive Processes</li>
	                <li>Principles of Data and System Security</li>
	            </ul>
	        </div>

	        <div style="float: right; width: 50%;">
	            <ul style="list-style: none;">
	            	<li><a href="https://www.bio.iitb.ac.in/people/faculty/srivastava-r/" target="_blank">Prof. Rohit Srivastava</a></li>
	            	<li><a href="https://indusj.wix.com/induiitb" target="_blank">Prof. Indu J</a></li>
	            	<li><a href="https://www.hss.iitb.ac.in/en/faculty-profile/rashmi-gupta" target="_blank">Prof. Rashmi Gupta</a></li>
	            	<li><a href="https://www.cse.iitb.ac.in/~rkss/" target="_blank">Prof. R.K. Shyamasundar</a></li>
	            </ul>
	        </div>

	        <div style="float: left; width: 100%;"><h3><p>Autumn 2017-18</p></h3></div>
	        <div style="float: left; width: 50%;">
	            <ul>
	                <li>Computer Graphics</li>
	                <li>Environmental Studies</li>
	                <li>Environmental Studies: Science and Engineering</li>
	                <li>Foundations of Intelligent Agents</li>
	                <li>Introduction to the Study of Language</li>
	                <li>Philosophy of Religion</li>
	            </ul>
	        </div>

	        <div style="float: right; width: 50%;">
	            <ul style="list-style: none;">
	                <li><a href="https://www.cse.iitb.ac.in/~paragc/" target="_blank">Prof. Parag Kumar Chaudhuri</a></li>
	                <li>Prof. Parameshwar B., <a href="https://www.hss.iitb.ac.in/en/faculty-profile/k-narayanan" target="_blank">Prof. Krishnan N.</a>, <a href="https://www.hss.iitb.ac.in/en/faculty-profile/neha-gupta" target="_blank">Prof. Neha Gupta</a></li>
	                <li><a href="https://www.esed.iitb.ac.in/oldwebsite/people/a.garg.php" target="_blank">Prof. Anurag Garg</a>, <a href="https://www.esed.iitb.ac.in/oldwebsite/people/phuleria.php" target="_blank">Prof. Harish Phuleria</a>, <a href="https://www.esed.iitb.ac.in/oldwebsite/people/sanjeev.php" target="_blank">Prof. Sanjeev C.</a></li>
	                <li><a href="https://www.cse.iitb.ac.in/~shivaram/" target="_blank">Prof. Shivaram Kalyankrishnan</a></li>
	                <li><a href="https://www.hss.iitb.ac.in/en/faculty-profile/vaijayanthi-sarma" target="_blank">Prof. Vaijayanthi M. Sarma</a></li>
	                <li>Prof. Parameshwar B., <a href="https://www.hss.iitb.ac.in/en/faculty-profile/pravesh-jung-golay" target="_blank">Prof. Pravesh J. Golay</a></li>
	            </ul>
	        </div>

	        <div style="float: left; width: 100%;"><h3><p>Spring 2016-17</p></h3></div>
	        <div style="float: left; width: 50%;">
	            <ul>
	                <li>Artificial Intelligence ( + lab)</li>
	                <li>Automata Theory</li>
	                <li>Foundations of Machine Learning</li>
	                <li>General Topology</li>
	                <li>Implementation of Programming Languages ( + lab)</li>
	                <li>Introduction to Numerical Analysis</li>
	            </ul>
	        </div>

	        <div style="float: right; width: 50%;">
	            <ul style="list-style: none;">
	                <li><a href="https://www.cse.iitb.ac.in/~shivaram/" target="_blank">Prof. Shivaram Kalyankrishnan</a></li>
	                <li><a href="https://www.cse.iitb.ac.in/~nutan/" target="_blank">Prof. Nutan Limaye</a></li>
	                <li><a href="https://www.cse.iitb.ac.in/~ganesh/" target="_blank">Prof. Ganesh Ramakrishnan</a></li>
	                <li><a href="https://sites.google.com/site/sandiptifr/" target="_blank">Prof. Sandip Singh</a></li>
	                <li><a href="https://www.cse.iitb.ac.in/~sb/" target="_blank">Prof. Supratim Biswas</a>, <a href="https://www.cse.iitb.ac.in/~uday/" target="_blank">Prof. Uday Khedker</a></li>
	                <li>Prof. Sivaji G. Sista, <a href="http://www.math.iitb.ac.in/~baskar/" target="_blank">Prof. S. Baskar</a></li>
	            </ul>
	        </div>

	        <div style="float: left; width: 100%;"><h3><p>Autumn 2016-17</p></h3></div>
	        <div style="float: left; width: 50%;">
	            <ul>
	                <li>Basic Algebra</li>
	                <li>Computer Architecture ( + lab)</li>
	                <li>Databases and Information Systems ( + lab)</li>
	                <li>Operating Systems ( + lab)</li>
	                <li>Psychology</li>
	            </ul>
	        </div>

	        <div style="float: right; width: 50%;">
	            <ul style="list-style: none;">
	            	<li><a href="http://www.math.iitb.ac.in/~reksan/" target="_blank">Prof. Rekha Santhanam</a></li>
	            	<li><a href="https://www.cse.iitb.ac.in/~umesh/index.html" target="_blank">Prof. Umesh R. Bellur</a></li>
	            	<li><a href="https://www.cse.iitb.ac.in/~sudarsha/" target="_blank">Prof. S Sudarshan</a></li>
	            	<li><a href="https://www.cse.iitb.ac.in/~mythili/" target="_blank">Prof. Mythili Vutukuru</a></li>
	            	<li><a href="https://www.hss.iitb.ac.in/en/faculty-profile/pooja-purang" target="_blank">Prof. Pooja Purang</a></li>
	            </ul>
	        </div>

	        <div style="float: left; width: 100%;"><h3><p>Spring 2015-16</p></h3></div>
	        <div style="float: left; width: 50%;">
	            <ul>
	                <li>Complex Analysis</li>
	                <li>Computer Networks ( + lab)</li>
	                <li>Design and Analysis of Algorithms</li>
	                <li>Digital Logic Design ( + lab)</li>
	                <li>Economics</li>
	                <li>Logic For Computer Science</li>
	            </ul>
	        </div>

	        <div style="float: right; width: 50%;">
	            <ul style="list-style: none;">
	                <li><a href="https://sites.google.com/site/sandiptifr/" target="_blank">Prof. Sandip Singh</a></li>
	            	<li><a href="https://www.cse.iitb.ac.in/~chebrolu/" target="_blank">Prof. Kameswari Chebrolu</a></li>
	                <li><a href="https://www.cse.iitb.ac.in/~ranade/" target="_blank">Prof. Abhiram G. Ranade</a></li>
	                <li><a href="https://www.cse.iitb.ac.in/~supratik/" target="_blank">Prof. Supratik Chakraborthy</a>, Prof. Ashwin Gumaste</li>
	                <li>Prof. Pushpa L. Trivedi, <a href="https://www.hss.iitb.ac.in/en/faculty-profile/puja-padhi" target="_blank">Prof. Puja Padhi</a></li>
	                <li><a href="https://www.cse.iitb.ac.in/~krishnas/" target="_blank">Prof. Krishna S.</a></li>
	            </ul>
	        </div>

	        <div style="float: left; width: 100%;"><h3><p>Autumn 2015-16</p></h3>
	        <div style="float: left; width: 50%;">
	            <ul>
	                <li>Algorithms and Data Structures ( + lab)</li>
	                <li>Data Analysis and Interpretation</li>
	                <li>Discrete Structures</li>
	                <li>Introduction to Electrical and Electronics Circuits</li>
	                <li>Real Analysis</li>
	                <li>Software Systems Lab</li>
	            </ul>
	        </div>

	        <div style="float: right; width: 50%;">
	            <ul style="list-style: none;">
	                <li><a href="https://www.cse.iitb.ac.in/~aad/" target="_blank">Prof. Ajit A. Diwan</a></li>
	                <li><a href="https://www.cse.iitb.ac.in/~ajitvr/" target="_blank">Prof. Ajit V. Rajwade</a>, <a href="https://www.cse.iitb.ac.in/~suyash/" target="_blank">Prof. Suyash P. Awate</a></li>
	                <li><a href="https://www.cse.iitb.ac.in/~akshayss/" target="_blank">Prof. S. Akshay</a></li>
	                <li><a href="https://www.ee.iitb.ac.in/wiki/faculty/slodha" target="_blank">Prof. Saurabh Lodha</a></li>
	                <li><a href="https://sites.google.com/view/pal-sourav/home" target="_blank">Prof. Sourav Pal</a></li>
	                <li><a href="https://www.cse.iitb.ac.in/~sharat/" target="_blank">Prof. Sharat Chandran</a></li>
	            </ul>
	        </div>
	        
	        <div style="float: left; width: 100%;"><h3><p>Spring 2014-15</p></h3></div>
	        <div style="float: left; width: 50%;">
	            <ul >
	                <li>Abstraction and Paradigm in Computer Programming (+ lab)</li>
	                <li>Basics of Electricity and Magnetism</li>
	                <li>Biology</li>
	                <li>Differential Equations</li>
	                <li>Linear Algebra</li>
	                <li>Mechanical Workshop</li>
	                <li>Physics Lab</li>
	            </ul>
	        </div>

	        <div style="float: right; width: 50%;">
	            <ul style="list-style: none;">
	                <li><a href="https://www.cse.iitb.ac.in/~damani/" target="_blank">Prof. Om P. Damani</a></li>
	                <br>
	                <li><a href="https://homepages.iitb.ac.in/~pradeepsarin/" target="_blank">Prof. Pradeep Sarin</a></li>
	                <li><a href="https://www.bio.iitb.ac.in/people/faculty/purwar-r/" target="_blank">Prof. Rahul Purwar</a>, <a href="https://www.bio.iitb.ac.in/people/faculty/srivastava-r/" target="_blank">Prof. Rohit Srivastava</a></li>
	                <li><a href="http://www.math.iitb.ac.in/~keshari/" target="_blank">Prof. Manoj Kumar Keshari</a></li>
	                <li><a href="http://www.math.iitb.ac.in/~keshari/" target="_blank">Prof. Manoj Kumar Keshari</a></li>
	                <li><a href="https://www.me.iitb.ac.in/?q=faculty/Prof.%20Amitava%20De" target="_blank">Prof. Amitava De</a></li>
	                <li><a href="https://sites.google.com/view/avmahajan/home" target="_blank">Prof. Avinash V. Mahajan</a></li>
	            </ul>
	        </div>

	        
	        <div style="float: left; width: 100%;"><h3><p>Autumn 2014-15</p></h3></div>
	        <div style="float: left; width: 50%;">
	            <ul>
	                <li>Chemistry Lab</li>
	                <li>Computer Programming and Utilization</li>
	                <li>Engineering Graphics & Drawing</li>
	                <li>Introduction to Calculus</li>
	                <li>Organic and Inorganic Chemistry</li>
	                <li>Physical Chemistry</li>
	                <li>Quantum Physics and Applications</li>
	            </ul>
	        </div>

	        <div style="float: right; width: 50%;">
	            <ul style="list-style: none;">
	                <li><a href="https://chemphysgrpiitb.wixsite.com/chemphysgrp/g-naresh-patwari" target="_blank">Prof. Naresh Patwari</a></li>
	                <li><a href="https://www.cse.iitb.ac.in/~supratik/" target="_blank">Prof. Supratik Chakraborthy</a>, <a href="https://www.cse.iitb.ac.in/~dbp/" target="_blank">Prof. Deepak B. Phatak</a></li>
	                <li><a href="https://www.me.iitb.ac.in/?q=faculty/Prof.%20Krishna%20Jonnalagadda" target="_blank">Prof. Krishna Jonnalagadda</a>, <a href="https://www.me.iitb.ac.in/~salil/" target="_blank">Prof. Salil S. Kulkarni</a></li>
	                <li><a href="http://www.math.iitb.ac.in/~ravir/" target="_blank">Prof. Ravi Raghunathan</a></li>
	                <li><a href="https://www.chem.iitb.ac.in/~pradeep/" target="_blank">Prof. PradeepKumar PI</a></li>
	                <li><a href="https://sandipkar8.wixsite.com/sandip-kar" target="_blank">Prof. Sandip Kar</a></li>
	                <li>Prof. Shiva Prasad</li>
	            </ul>
	        </div>
	        * : Current Courses
	    </div>
	<br>

</div>
