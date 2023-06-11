# Deep Learning
<p><b>1. Overview</b><span style="font-weight: 400;">: Purpose of this analysis.</span></p>
<p><span style="font-weight: 400;">The purpose of this analysis was to determine whether funding provided by Alphabet Soup to different applicants will result in the execution of a successful venture or not. What success means is not clearly defined, but it is indicated as a boolean variable. However, defining success differently (such as achieving certain valuation for their venture) might result in a higher quality model.</span></p>
<p><span style="font-weight: 400;">Furthermore, the income is provided as a range, while the asked amount is provided as a number. My opinion is that utilizing a number for income instead of a range would result in a higher quality model. </span></p>
<br></br>
<ol>
<p><b>2. Results</b><span style="font-weight: 400;">: Using bulleted lists and images to support your answers, address the following questions:</span></p>
</ol>
<ul>
<li style="font-weight: 400;" aria-level="1"><span style="font-weight: 400;">Data Preprocessing</span></li>
<ul>
<li style="font-weight: 400;" aria-level="2"><span style="font-weight: 400;">What variable(s) are the target(s) for your model?</span></li>
<ul>
<li style="font-weight: 400;" aria-level="3"><span style="font-weight: 400;">Target:</span></li>
<ul>
<li style="font-weight: 400;" aria-level="4"><span style="font-weight: 400;">IS_SUCCESSFUL</span></li>
</ul>
</ul>
<li style="font-weight: 400;" aria-level="2"><span style="font-weight: 400;">What variable(s) are the features for your model?</span>
<ul>
<li style="font-weight: 400;" aria-level="3"><span style="font-weight: 400;">The features are:</span>
<ul>
<li style="font-weight: 400;" aria-level="4"><span style="font-weight: 400;">APPLICATION_TYPE</span></li>
<li style="font-weight: 400;" aria-level="4"><span style="font-weight: 400;">AFFILIATION</span></li>
<li style="font-weight: 400;" aria-level="4"><span style="font-weight: 400;">CLASSIFICATION</span></li>
<li style="font-weight: 400;" aria-level="4"><span style="font-weight: 400;">USE_CASE</span></li>
<li style="font-weight: 400;" aria-level="4"><span style="font-weight: 400;">ORGANIZATION</span></li>
<li style="font-weight: 400;" aria-level="4"><span style="font-weight: 400;">STATUS</span></li>
<li style="font-weight: 400;" aria-level="4"><span style="font-weight: 400;">INCOME_AMT</span></li>
<li style="font-weight: 400;" aria-level="4"><span style="font-weight: 400;">SPECIAL_CONSIDERATIONS</span></li>
<li style="font-weight: 400;" aria-level="4"><span style="font-weight: 400;">ASK_AMT</span></li>
</ul>
</li>
</ul>
</li>
<li><span style="font-weight: 400;">What variable(s) should be removed from the input data because they are neither targets nor features?</span>
<ul>
<li><span style="font-weight: 400;">Neither targets nor features:</span>
<ul>
<li style="font-weight: 400;" aria-level="4"><span style="font-weight: 400;">EIN</span></li>
<li style="font-weight: 400;" aria-level="4"><span style="font-weight: 400;">NAME</span></li>
</ul>
</li>
</ul>
</li>
<li><span style="font-weight: 400;">Compiling, Training, and Evaluating the Model</span>
<ul>
<li><span style="font-weight: 400;">How many neurons, layers, and activation functions did you select for your neural network model, and why?</span>
<ul>
<li style="font-weight: 400;" aria-level="3"><span style="font-weight: 400;">Neurons: 129; it&rsquo;s the recommended amount of 2-3 times the amount of features (43).</span></li>
<li style="font-weight: 400;" aria-level="3"><span style="font-weight: 400;">Layers: 2 hidden layers + 1 output layer; started with 2, then did 3 without seeing significant improvement.</span></li>
<li style="font-weight: 400;" aria-level="3"><span style="font-weight: 400;">Activation functions:</span>
<ul>
<li style="font-weight: 400;" aria-level="4"><span style="font-weight: 400;">Hidden layer 1: relu; it&rsquo;s better to use more complex functions for hidden layers.</span></li>
<li style="font-weight: 400;" aria-level="4"><span style="font-weight: 400;">Hidden layer 2: relu</span></li>
<li style="font-weight: 400;" aria-level="4"><span style="font-weight: 400;">Output layer: tanh; tanh was slightly better than sigmoid.</span></li>
</ul>
</li>
</ul>
</li>
</ul>
</li>
<li><span style="font-weight: 400;">Were you able to achieve the target model performance?</span>
<ul>
<li><span style="font-weight: 400;">No, the accuracy stayed at around 74%. My guess is that the data isn&rsquo;t of enough quality.</span></li>
</ul>
</li>
<li><span style="font-weight: 400;">What steps did you take in your attempts to increase model performance?</span>
<ul>
<li><span style="font-weight: 400;">I added 2 more layers</span></li>
<li><span style="font-weight: 400;">I added more neurons</span></li>
<li><span style="font-weight: 400;">I removed 2 columns (Classification and Application Type): This negatively affected accuracy but not for a lot, which means these features don&rsquo;t explain a big part of the outcome.<br /></span></li>
</ul>
</li>
</ul>
</ul>
