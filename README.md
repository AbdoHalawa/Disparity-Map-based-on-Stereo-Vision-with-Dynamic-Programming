<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Disparity Map based on Stereo Vision with Dynamic Programming</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 20px;
        }
        h1, h2 {
            color: #333;
        }
        pre {
            background-color: #f4f4f4;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
    </style>
</head>
<body>

<h1>Disparity Map based on Stereo Vision with Dynamic Programming</h1>

<p>This project implements a method to estimate the disparity map and depth information using Dynamic Programming (DP) on stereo vision images. The benchmark Middlebury database is used for testing and comparison with ground truth data.</p>

<h2>Table of Contents</h2>
<ul>
    <li><a href="#introduction">Introduction</a></li>
    <li><a href="#features">Features</a></li>
    <li><a href="#requirements">Requirements</a></li>
    <li><a href="#installation">Installation</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#examples">Examples</a></li>
    <li><a href="#results">Results</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
</ul>

<h2 id="introduction">Introduction</h2>
<p>Stereo vision is a technique for recovering depth from two cameras with known relative positions. This project focuses on applying Dynamic Programming to stereo vision images to generate a disparity map, which is then used to infer depth information. The output is compared against ground truth data from the Middlebury database to evaluate performance.</p>

<h2 id="features">Features</h2>
<ul>
    <li>Estimate disparity map using Dynamic Programming.</li>
    <li>Calculate depth information from stereo images.</li>
    <li>Compare results with ground truth from the Middlebury database.</li>
</ul>

<h2 id="requirements">Requirements</h2>
<ul>
    <li>Python 3.6+</li>
    <li>NumPy</li>
    <li>OpenCV</li>
    <li>Matplotlib</li>
    <li>Middlebury Stereo Datasets</li>
</ul>

<h2 id="installation">Installation</h2>
<ol>
    <li>Clone the repository:
        <pre><code>git clone https://github.com/your-username/disparity-map-dynamic-programming.git
cd disparity-map-dynamic-programming</code></pre>
    </li>
    <li>Install the required packages:
        <pre><code>pip install -r requirements.txt</code></pre>
    </li>
</ol>

<h2 id="usage">Usage</h2>
<ol>
    <li>Place the left and right images from the Middlebury dataset in the <code>data/</code> directory.</li>
    <li>Run the script to compute the disparity map:
        <pre><code>python disparity_map.py --left data/left_image.png --right data/right_image.png</code></pre>
    </li>
</ol>

<h3>Command Line Arguments</h3>
<ul>
    <li><code>--left</code>: Path to the left image.</li>
    <li><code>--right</code>: Path to the right image.</li>
</ul>

<h2 id="examples">Examples</h2>
<pre><code>python disparity_map.py --left data/left_image.png --right data/right_image.png</code></pre>

<h2 id="results">Results</h2>
<p>The disparity map and depth information will be saved in the <code>output/</code> directory. Additionally, the script will display the computed disparity map and the comparison with the ground truth.</p>

<h2 id="contributing">Contributing</h2>
<p>Contributions are welcome! Please feel free to submit a Pull Request.</p>

<h2 id="license">License</h2>
<p>This project is licensed under the MIT License. See the <a href="LICENSE">LICENSE</a> file for more details.</p>

<h2 id="acknowledgments">Acknowledgments</h2>
<ul>
    <li>The Middlebury Stereo Vision Research Page for providing the datasets.</li>
    <li><a href="https://opencv.org/">OpenCV</a> and <a href="https://numpy.org/">NumPy</a> for their amazing tools and libraries.</li>
</ul>

</body>
</html>
