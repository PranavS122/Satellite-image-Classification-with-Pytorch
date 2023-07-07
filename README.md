<h1>Satellite Image Classification with PyTorch</h1>

<h2>Introduction</h2>

<h4>Basic Idea for the Project</h4>

<p>Satellite image classification can be used for environmental monitoring and assessment, allowing businesses to analyze the state of different areas of land from a remote location.</p>
<p>The classification model can support land management and urban planning by identifying regions suitable for development, preservation, or conservation.</p>
<p>It enables monitoring of natural resources such as water bodies, forests, and agricultural land, aiding in the identification of potential issues or changes over time.</p>
<p>The model can assist in disaster management by quickly assessing the impact of natural disasters like wildfires, floods, or storms on different land areas.</p>
<p>Industries like agriculture, forestry, and renewable energy can benefit from satellite image classification by optimizing resource allocation and decision-making processes based on the classification results.</p>

<h2>Dataset Information</h2>

<p>The dataset is a compressed RAR file created by subsetting the Satellite Dataset from Kaggle.</p>
<p>You can access the dataset from this Kaggle link: <a href="https://www.kaggle.com/datasets/mahmoudreda55/satellite-image-classification">Satellite Image Classification Dataset</a>.</p>
<p>The dataset consists of images categorized into four classes: desert, green area, cloudy, and water.</p>
<p>It includes a total of 500 training images, 150 testing images, and 50 validation images.</p>

<h2>Model Training and Deployment</h2>

<p>The model used for this project is VGG16, a popular convolutional neural network architecture.</p>
<p>Here are the training statistics:</p>

<table>
  <tr>
    <th>Epoch</th>
    <th>Last Learning Rate</th>
    <th>Training Loss</th>
    <th>Validation Accuracy</th>
    <th>Validation Loss</th>
  </tr>
  <tr>
    <td>0</td>
    <td>0.00271</td>
    <td>0.6527</td>
    <td>0.9651</td>
    <td>0.2368</td>
  </tr>
  <tr>
    <td>1</td>
    <td>0.00755</td>
    <td>0.1025</td>
    <td>0.9828</td>
    <td>0.0812</td>
  </tr>
  <tr>
    <td>2</td>
    <td>0.01000</td>
    <td>0.0497</td>
    <td>0.9891</td>
    <td>0.0537</td>
  </tr>
  <tr>
    <td>3</td>
    <td>0.00950</td>
    <td>0.0443</td>
    <td>0.9953</td>
    <td>0.0341</td>
  </tr>
  <tr>
    <td>4</td>
    <td>0.00812</td>
    <td>0.0276</td>
    <td>0.9922</td>
    <td>0.0356</td>
  </tr>
  <tr>
    <td>5</td>
    <td>0.00611</td>
    <td>0.0366</td>
    <td>0.9922</td>
    <td>0.0308</td>
  </tr>
  <tr>
    <td>6</td>
    <td>0.00389</td>
    <td>0.0274</td>
    <td>0.9937</td>
    <td>0.0325</td>
  </tr>
  <tr>
    <td>7</td>
    <td>0.00188</td>
    <td>0.0290</td>
    <td>0.9922</td>
    <td>0.0297</td>
  </tr>
  <tr>
    <td>8</td>
    <td>0.00050</td>
    <td>0.0298</td>
    <td>0.9937</td>
    <td>0.0276</td>
  </tr>
  <tr>
    <td>9</td>
    <td>0.00000</td>
    <td>0.0200</td>
    <td>0.9937</td>
    <td>0.0273</td>
  </tr>
</table>

<h2>Model Deployment</h2>

<p>The trained model was deployed using Gradio, a Python library for creating UIs around machine learning models.</p>
<p>With the deployed model, you can interactively classify satellite images and observe the predicted class.</p>
