

<div class="Section1">

<p class="MsoNormal" align="center" style="text-align: center;"><b style=""><span style="font-size: 18pt; line-height: 115%; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">SFND
RADAR Target Generation and Detection<o:p></o:p></span></b></p>

<p class="MsoNormal"><span style="font-size: 12pt; line-height: 115%; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">In this project, RADAR will be used to
detect target by filtering the noise. <span style="">&nbsp;</span>This can be achieved using following steps<o:p></o:p></span></p>

<p class="MsoNormal"><span style="font-size: 12pt; line-height: 115%; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><img width="624" height="329" src="imgs/image002.gif" alt="project_layout.png" v:shapes="Picture_x0020_0"></span><span style="font-size: 12pt; line-height: 115%; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><o:p></o:p></span></p>

<ol start="1" type="1">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Configure the FMCW waveform
     based on the system requirements.<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); margin-top: 3pt; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Define the range and velocity
     of target and simulate its displacement.<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); margin-top: 3pt; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">For the same simulation loop
     process the transmit and receive signal to determine the beat signal.<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); margin-top: 3pt; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Perform Range FFT on the
     received signal to determine the Range.<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); margin-top: 3pt; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Towards the end, perform the
     CFAR processing on the output of 2nd FFT to display the target.<o:p></o:p></span></li>
</ol>

<h1><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">RADAR Specifications:<o:p></o:p></span></h1>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Frequency of operation = 77GHz<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); margin-top: 3pt; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Max Range = 200m<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); margin-top: 3pt; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Range Resolution = 1 m<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); margin-top: 3pt; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Max Velocity = 100 m/s<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-top: 3pt; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="200" height="77" src="imgs/image004.jpg" v:shapes="Picture_x0020_4"></span><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></p>

<h2><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">User Defined Range and
Velocity of target:<o:p></o:p></span></h2>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Defined Velocity and Range of
     Target<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-left: 0.25in; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="173" height="55" src="imgs/image006.jpg" v:shapes="Picture_x0020_10"></span><b style=""><u><span style="font-size: 16pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></u></b></p>

<h2><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">FMCW Waveform Design:</span><span style="font-size: 12pt; line-height: 115%; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><o:p></o:p></span></h2>

<ul type="disc">
 <li class="MsoNormal" style="line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);">Designed FMCW
     waveform using the given system requirements. Calculated Bandwidth (B),
     Chirp Time (Tchirp) and Slope (slope).</span><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-top: 3pt; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="345" height="84" src="imgs/image008.jpg" v:shapes="Picture_x0020_13"></span><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></p>

<p class="MsoNormal" style="margin-top: 3pt; text-indent: 0.5in; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);">Got slope value as 2.045e+13.<o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Defined operating carrier
     frequency of Radar as per specification<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="78" height="27" src="imgs/image010.jpg" v:shapes="Picture_x0020_16"></span><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Number of Chirps value is set as
     128 in one sequence as its ideal to have 2^ value for the ease of running
     FFT for Doppler Estimation.<span style="">&nbsp; </span>Defined
     number of samples on each chirp as 1024.<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-left: 0.25in; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="624" height="62" src="imgs/image012.jpg" v:shapes="Picture_x0020_19"></span><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Timestamp for running the
     displacement scenario for every sample on each chirp<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-left: 0.25in; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="246" height="20" src="imgs/image014.jpg" v:shapes="Picture_x0020_22"></span><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Defining the vectors for Tx, Rx
     and Mix based on the total samples input.<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-left: 0.25in; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="343" height="66" src="imgs/image016.jpg" v:shapes="Picture_x0020_25"></span><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></p>

<p class="MsoNormal" style="margin-left: 0.5in; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p>&nbsp;</o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Similar vectors for
     range_covered and time delay.<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-left: 0.25in; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="188" height="46" src="imgs/image018.jpg" v:shapes="Picture_x0020_28"></span><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></p>

<h2><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Signal generation and
Moving Target simulation:<o:p></o:p></span></h2>

<p class="MsoNormal" align="center" style="text-align: center;"><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><img width="624" height="197" src="imgs/image020.jpg" v:shapes="Picture_x0020_34"></span><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Generated Signal and simulated
     the moving target which is defined initially. Updated transmitted and
     received signal values based on the formulae.<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="text-align: center;"><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><img width="624" height="329" src="imgs/image022.jpg" v:shapes="Picture_x0020_31"></span><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><o:p></o:p></span></p>

<h2><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">RANGE MEASUREMENT:<o:p></o:p></span></h2>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Reshape the vector into Nr * Nd
     array<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-left: 0.5in; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><img width="248" height="22" src="imgs/image024.jpg" v:shapes="Picture_x0020_37"></span><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Run the FFT on the beat signal
     along the range bins dimension (Nr) <o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-left: 0.5in; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="187" height="28" src="imgs/image026.jpg" v:shapes="Picture_x0020_40"></span><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Take the absolute value of FFT
     output and normalize<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-left: 0.5in; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="256" height="43" src="imgs/image028.jpg" v:shapes="Picture_x0020_43"></span><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Output of FFT is double sided
     signal, but we are interested in only one side of the spectrum. Hence we
     throw out half of the samples.<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-left: 0.5in; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="278" height="23" src="imgs/image030.jpg" v:shapes="Picture_x0020_46"></span><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Plotting of FFT Output<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-left: 0.5in; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="164" height="37" src="imgs/image032.jpg" v:shapes="Picture_x0020_49"></span><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Simulation Result is as follows</span><b style=""><u><span style="font-size: 16pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><img width="552" height="189" src="imgs/image034.jpg" alt="1.jpg" v:shapes="Picture_x0020_1"></span></u></b><b style=""><u><span style="font-size: 16pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><o:p></o:p></span></u></b></li>
</ul>

<h2><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">RANGE DOPPLER RESPONSE:<o:p></o:p></span></h2>

<h3><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Range Doppler Map
Generation:<o:p></o:p></span></h3>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Output of 2D FFT is an image
     that has response in the range and Doppler FFT bins. So, it is important
     to convert the axis from bin sizes to range and Doppler based on their Max
     values.<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><img width="193" height="42" src="imgs/image036.jpg" v:shapes="Picture_x0020_55"></span><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">2D FFT using the FFT size
     dimensions for both <o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="text-align: center;"><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><img width="226" height="40" src="imgs/image038.jpg" v:shapes="Picture_x0020_58"></span><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Taking just one side of signal
     from Range dimension<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-left: 0.25in; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><img width="263" height="74" src="imgs/image040.jpg" v:shapes="Picture_x0020_61"></span><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Use the surf function to plot
     the output of 2DFFT and to show axis in both dimensions<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><img width="411" height="63" src="imgs/image042.jpg" v:shapes="Picture_x0020_64"></span><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);">Output of 2D FFT
     is as follows</span><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><o:p></o:p></span></li>
</ul>

<p class="MsoNormal" style="margin-top: 3pt; line-height: normal; background-color: white; background-image: initial;"><b style=""><u><span style="font-size: 16pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="544" height="408" src="imgs/image043.jpg" alt="2.jpg" v:shapes="Picture_x0020_2"></span></u></b><b style=""><u><span style="font-size: 16pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></u></b></p>

<h2>CFAR implementation:</h2>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Determined the number of
     training cells for each dimension Tr and Td. Similarly, picked the number
     for guard cells Gr and Gd.<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Defined Grid Size and Train
     Cells based on both Leading and Trailing cells. So, multiplied by 2.<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="426" height="43" src="imgs/image045.jpg" v:shapes="Picture_x0020_82"></span><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Designed a loop such that it
     slides the CUT across Range Doppler Map<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Slide the cell under test (CUT)
     across the complete cell matrix.<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">For every iteration sum the
     signal level within all the training cells. To sum convert the value from
     logarithmic to linear using db2pow function.<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Average the summed values for
     all of the training cells used. After averaging convert it back to
     logarithmic using pow2db.<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Further added the offset to it
     to determine the threshold.<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Compare the signal under CUT
     against this threshold.<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">If the CUT level &gt; threshold
     assign it a value of 1, else equate it to 0.<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="text-align: center;"><span style=""><img width="520" height="460" src="imgs/image047.jpg" v:shapes="Picture_x0020_85"></span></p>

<h2>Selection of Training, Guard cells and offset.</h2>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Number of Training cells in Range
     dimension (Tr) = 10<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Number of Training cells in Doppler
     dimension (Td) = 8<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-top: 3pt; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-family: &quot;Segoe UI&quot;, &quot;sans-serif&quot;; color: rgb(36, 41, 46);"><img width="75" height="42" src="imgs/image049.jpg" v:shapes="Picture_x0020_67"></span><span style="font-family: &quot;Segoe UI&quot;, &quot;sans-serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Number of Guard cells in Range
     dimension (Gr) = 4<o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Number of Guard cells in Doppler
     dimension (Gd) = 4<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-left: 0.25in; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="71" height="39" src="imgs/image051.jpg" v:shapes="Picture_x0020_70"></span><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">Offset the threshold by SNR
     value in dB. Offset = 1.4.<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="text-align: center;"><span style=""><img width="112" height="24" src="imgs/image053.jpg" v:shapes="Picture_x0020_73"></span></p>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">These values are chosen by
     observing iteratively..<o:p></o:p></span></li>
</ul>

<h2><span style="background-color: white; background-image: initial;">Steps taken to suppress the Non- Thresholded
cells at the edges:<o:p></o:p></span></h2>

<ul type="disc">
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">The process above will generate
     a thresholded block, which is smaller than the Range Doppler Map (RDM) as
     the Cell Under Test (CUT) cannot be located at the edges of matrix.So, few
     cells will not be thresholded. To keep the map size same set those values
     to 0. <o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">So, locating the indices where
     threshold is not applied and setting the value to 0. <o:p></o:p></span></li>
 <li class="MsoNormal" style="color: rgb(36, 41, 46); line-height: normal; background-color: white; background-image: initial;"><span style="font-size: 12pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;">If CUT is less than threshold,
     we have set value to zero and else 1. So, checking the indices where value
     is neither 0 nor 1 and setting them 0 with following statement<o:p></o:p></span></li>
</ul>

<p class="MsoNormal" align="center" style="margin-left: 0.25in; text-align: center; line-height: normal; background-color: white; background-image: initial;"><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><img width="241" height="36" src="imgs/image055.jpg" v:shapes="Picture_x0020_76"></span><span style="font-family: &quot;Times New Roman&quot;, &quot;serif&quot;;"><o:p></o:p></span></p>

<h2>CFAR Output:</h2>

<p class="MsoNormal" style="margin-top: 3pt; line-height: normal; background-color: white; background-image: initial;"><b style=""><u><span style="font-size: 16pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><img width="506" height="294" src="imgs/image057.jpg" alt="3.jpg" v:shapes="Picture_x0020_3"></span></u></b><b style=""><u><span style="font-size: 16pt; font-family: &quot;Times New Roman&quot;, &quot;serif&quot;; color: rgb(36, 41, 46);"><o:p></o:p></span></u></b></p>

</div>




