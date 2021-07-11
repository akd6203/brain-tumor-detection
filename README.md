# brain tumor detection using python and sklearn

<!-- wp:image {"id":21,"sizeSlug":"large","linkDestination":"none","style":{"color":[]}} -->
<figure class="wp-block-image size-large"><img src="https://cwadtech.files.wordpress.com/2021/07/istockphoto-939518752-612x612-1.jpg?w=612" alt="" class="wp-image-21"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Hii Readers, In this post we are going to learn about brain tumor detection using sklearn and python.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Requirements:</h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>python (<a href="https://www.python.org/downloads/"><em>https://www.python.org/downloads/</em></a>)</li><li>sklearn (<em>pip install sklearn</em>)</li><li>openCV (<em>pip install opencv-python</em>)</li><li>numpy (<em>pip install numpy</em>)</li><li>matplotlib (<em>pip install matplotlib</em>)</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3>DOWNLOAD CODE :</h3>
<!-- /wp:heading -->

<!-- wp:list {"ordered":true} -->
<ol><li>Download the code from github</li><li>Download all above mentioned dependencies.</li><li>Open downloaded folder inside jupyter notebook.</li><li>Now cells as per your requirements.</li></ol>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3>STEP 1: Load Dependencies</h3>
<!-- /wp:heading -->

<!-- wp:image {"align":"left","id":24,"sizeSlug":"large","linkDestination":"none"} -->
<div class="wp-block-image"><figure class="alignleft size-large"><img src="https://cwadtech.files.wordpress.com/2021/07/img.png?w=680" alt="" class="wp-image-24"/></figure></div>
<!-- /wp:image -->

<!-- wp:heading {"level":3} -->
<h3>STEP 2: Load and prepare data</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Note: You can find dataset directory inside github repository link (given below) or download dataset from  <a href="https://www.kaggle.com/sartajbhuvaji/brain-tumor-classification-mri" data-type="URL" data-id="https://www.kaggle.com/sartajbhuvaji/brain-tumor-classification-mri">kaggle</a></p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":25,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image size-large"><img src="https://cwadtech.files.wordpress.com/2021/07/img-1.png?w=680" alt="" class="wp-image-25"/></figure>
<!-- /wp:image -->

<!-- wp:heading {"level":3} -->
<h3>STEP 3: Data Analysis</h3>
<!-- /wp:heading -->

<!-- wp:image {"id":28,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image size-large"><img src="https://cwadtech.files.wordpress.com/2021/07/img-2.png?w=681" alt="" class="wp-image-28"/></figure>
<!-- /wp:image -->

<!-- wp:heading {"level":3} -->
<h3>STEP 4: Data Visualization</h3>
<!-- /wp:heading -->

<!-- wp:image {"id":29,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image size-large"><img src="https://cwadtech.files.wordpress.com/2021/07/img-3.png?w=680" alt="" class="wp-image-29"/></figure>
<!-- /wp:image -->

<!-- wp:heading {"level":3} -->
<h3>STEP 5: Split Data</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>In this step, we are going to split data in two parts (training and testing), so that we can train our model on training dataset and test its accuracy on unseen (test) data.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":30,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image size-large"><img src="https://cwadtech.files.wordpress.com/2021/07/img-4.png?w=760" alt="" class="wp-image-30"/></figure>
<!-- /wp:image -->

<!-- wp:heading -->
<h2>STEP 6: Feature Scaling</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>In this step, we are going to use minmax scaling technique to bring all the feature values to less than or equal to 1. In order to do so, we have divided the training data by its maximum value.</p>
<!-- /wp:paragraph -->

<!-- wp:gallery {"ids":[31],"linkTo":"none"} -->
<figure class="wp-block-gallery columns-1 is-cropped"><ul class="blocks-gallery-grid"><li class="blocks-gallery-item"><figure><img src="https://cwadtech.files.wordpress.com/2021/07/img-5.png?w=681" alt="" data-id="31" data-link="https://cwadtech.wordpress.com/img-5/" class="wp-image-31"/></figure></li></ul></figure>
<!-- /wp:gallery -->

<!-- wp:heading {"level":3} -->
<h3>STEP 7: Model Training</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>As we have done with preprocessing part, it is time to train our model. I am going to train model using SVM (Support Vector Machine) and Logistic Regression algorithms and then we will compare the performance of these two different models.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":35,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image size-large"><img src="https://cwadtech.files.wordpress.com/2021/07/img-7.png?w=681" alt="" class="wp-image-35"/></figure>
<!-- /wp:image -->

<!-- wp:heading {"level":3} -->
<h3>STEP 8: Evaluation</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>In this part, we will compare the scores of above two models.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":36,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image size-large"><img src="https://cwadtech.files.wordpress.com/2021/07/img-8.png?w=680" alt="" class="wp-image-36"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>As we can observe, <strong>SVM </strong>showed a great balance among training an testing score as compared to Logistic Regression. So we can reach to the conclusion that it is ideal model for this particular dataset</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>STEP 9: Prediction</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>In this step we are going to predict test dataset. Afterwards, I have checked the total number of misclassified samples out of total test samples.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":41,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image size-large"><img src="https://cwadtech.files.wordpress.com/2021/07/img-9.png?w=680" alt="" class="wp-image-41"/></figure>
<!-- /wp:image -->

<!-- wp:heading {"level":3} -->
<h3>STEP 10: TESTING (On test dataset)</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Finally, it is the time to examine the results.</p>
<!-- /wp:paragraph -->

<!-- wp:gallery {"ids":[46,47],"linkTo":"none"} -->
<figure class="wp-block-gallery columns-2 is-cropped"><ul class="blocks-gallery-grid"><li class="blocks-gallery-item"><figure><img src="https://cwadtech.files.wordpress.com/2021/07/img-11.png?w=680" alt="" data-id="46" data-link="https://cwadtech.wordpress.com/img-11/" class="wp-image-46"/></figure></li><li class="blocks-gallery-item"><figure><img src="https://cwadtech.files.wordpress.com/2021/07/img-12.png?w=655" alt="" data-id="47" data-full-url="https://cwadtech.files.wordpress.com/2021/07/img-12.png" data-link="https://cwadtech.wordpress.com/img-12/" class="wp-image-47"/></figure></li></ul></figure>
<!-- /wp:gallery -->

<!-- wp:heading {"level":4} -->
<h4>OUTPUT</h4>
<!-- /wp:heading -->

<!-- wp:gallery {"ids":[49,50],"linkTo":"none"} -->
<figure class="wp-block-gallery columns-2 is-cropped"><ul class="blocks-gallery-grid"><li class="blocks-gallery-item"><figure><img src="https://cwadtech.files.wordpress.com/2021/07/img-13.png?w=649" alt="" data-id="49" data-link="https://cwadtech.wordpress.com/img-13/" class="wp-image-49"/></figure></li><li class="blocks-gallery-item"><figure><img src="https://cwadtech.files.wordpress.com/2021/07/img-14.png?w=639" alt="" data-id="50" data-full-url="https://cwadtech.files.wordpress.com/2021/07/img-14.png" data-link="https://cwadtech.wordpress.com/img-14/" class="wp-image-50"/></figure></li></ul></figure>
<!-- /wp:gallery -->

<!-- wp:paragraph -->
<p>So, this is all about creating a predictive model using sklearn on brain tumor dataset. Thanks for reading!</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p></p>
<!-- /wp:paragraph -->
