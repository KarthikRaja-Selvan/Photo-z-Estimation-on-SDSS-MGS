<h1>Photometric Redshift Estimation using Main Galaxy Sample (MGS) from Sloan Digital Sky Survey (SDSS)</h1>

<h2>Project Overview</h2>

<p>In this project, I explore photometric redshift (photo-z) estimation using machine learning, with data drawn from the Main Galaxy Sample (MGS) in the Sloan Digital Sky Survey (SDSS) Data Release 18. The focus is on improving photo-z estimation accuracy by experimenting with different input parameters and configurations.</p>

<p>Key research questions addressed in this analysis:</p>
<ol>
    <li><strong>Effect of Band Reduction</strong>: How does the accuracy of photometric redshift estimation change when the number of photometric bands is reduced?</li>
    <li><strong>Inclusion of Band Magnitude Error</strong>: What is the impact on photo-z accuracy when band magnitude errors are included in the model input?</li>
    <li><strong>Band Contribution</strong>: Which photometric band (among U, G, R, I, Z) degrades the accuracy of photo-z estimation the most?</li>
    <li><strong>Inclusion of Morphological Parameters</strong>: How does adding morphological information improve or affect the accuracy of photo-z estimation?</li>
</ol>

<h2>Dataset</h2>

<p>The data used in this project is taken from the <strong>SDSS Data Release 18 (DR18)</strong>. Specifically, the photometric measurements and corresponding morphological parameters of galaxies in the Main Galaxy Sample (MGS) are used as input for training and evaluating machine learning models.</p>

<h2>Machine Learning Model</h2>

<p>For the estimation of photometric redshifts, I have used the <strong>RandomForestRegressor</strong> from the scikit-learn library, with its default configuration:</p>

<pre>
<code>sklearn.ensemble.RandomForestRegressor(
    n_estimators=100,
    criterion='squared_error',
    max_depth=None,
    min_samples_split=2,
    min_samples_leaf=1,
    max_features=1.0,
    bootstrap=True
)</code>
</pre>

<h2>Goals</h2>

<ul>
    <li>To improve the accuracy of photometric redshift estimation by optimizing the input features.</li>
    <li>To identify which photometric bands and parameters most significantly affect the estimation process.</li>
</ul>
