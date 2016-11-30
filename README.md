# news-events-tabs

In this tutorial, [Solodev](https://www.solodev.com/) shows how to add news and event listings in a tabbed module. In doing so, you will be able to display all necessary information in specific sections that could not otherwise display the content..

## Tutorial

For detailed instructions, view Solodev's [Adding News & Events Tabs](https://www.solodev.com/blog/web-design/adding-news-events-tabs.stml) article.

## Demo

Try out a working example on [JSFiddle](https://jsfiddle.net/solodev/m8qzqve1/).

## HTML

The tabs are based on default Bootstrap components and the following HTML:

```
<div class="container">  

  <h3>EVENTS & NEWS</h3>
  
  <hr>
  <div class="row">
    <div class="col-lg-push-4 col-md-4 col-md-push-4">
      <div class="searchForm type2">
        <form action="" class="searchForm"><!-- Add The Appropriate Action for Your Site's Search Form/Page -->
          <label class="sr-only" for="searchNewsEvents">Search News and Events</label>
           <input id="searchNewsEvents" name="q" placeholder="What are you looking for?" type="search"> <input type="submit" value="Search">
        </form>
      </div>
    </div>
    <div class="clearfix visible-sm visible-xs">
      &nbsp;
    </div>
    <div class="col-lg-push-4 col-md-4 col-md-push-4">
      <div class="dropdownCategories">
      <label class="sr-only" for="dropdownNewsEvents">Category dropdown for News and Events</label>
      <select>
        <option value="">
          Select Category
        </option>
        <option value=""><!-- Each option value should correspond to the appropriate filter on your site's News or Events page -->
          Marketing
        </option>
        <option value=""><!-- Each option value should correspond to the appropriate filter on your site's News or Events page -->
          Design
        </option>
        <option value=""><!-- Each option value should correspond to the appropriate filter on your site's News or Events page -->
          Programming
        </option>
        <option value=""><!-- Each option value should correspond to the appropriate filter on your site's News or Events page -->
          Support
        </option>
        <option value=""><!-- Each option value should correspond to the appropriate filter on your site's News or Events page -->
          Training
        </option>
      </select>
      </div>
    </div>  
    <div class="clearfix visible-sm visible-xs">
      &nbsp;
    </div>
    <div class="col-lg-4 col-lg-pull-8 col-md-4 col-md-pull-8">
      <ul class="nav nav-pills" role="tablist">
        <li class="active">
          <a data-toggle="tab" href="#tab1" role="tab">Events</a>
        </li>
        <li>
          <a data-toggle="tab" href="#tab2" role="tab">News</a>
        </li>
      </ul>
    </div>
  </div><!-- / row -->
  <hr>
  <div class="tab-content">
    <div class="tab-pane fade in active" id="tab1">
      <div class="row">
        <div class="col-md-6">
          <div class="media">
            <a class="pull-left" href="#"><span class="dateEl"><em>30</em>Nov</span></a>
            <div class="media-body">
              <h4 class="media-heading">
                <a href="#">Venture Tech</a>
              </h4>
              <div class="meta-data">
                <span class="longDate">Nov 30, 2016</span> <span class="timeEl">12:00pm - 02:00pm</span>
              </div>
              <p>
                See the latest inspirations in the local tech scene.
              </p>
            </div><!-- / media-body -->
          </div><!-- / media -->
          <div class="media">
            <a class="pull-left" href="#"><span class="dateEl"><em>11</em>Dec</span></a>
            <div class="media-body">
              <h4 class="media-heading">
                <a href="#">Tech Conference</a>
              </h4>
              <div class="meta-data">
                <span class="longDate">Dec 11, 2016</span> <span class="timeEl">06:00pm - 07:30pm</span>
              </div>
              <p>
                Local tech entrepreneurs gather to share their knowledge.
              </p>
            </div><!-- / media-body -->
          </div><!-- / media -->
          <div class="media">
            <a class="pull-left" href="#"><span class="dateEl"><em>15</em>Dec</span></a>
            <div class="media-body">
              <h4 class="media-heading">
                <a href="#">Marketing for Large Businesses</a>
              </h4>
              <div class="meta-data">
                <span class="longDate">Dec 15, 2016</span> <span class="timeEl">05:30pm - 07:30pm</span>
              </div>
              <p>
                Learn how larger organizations can effectively manager their marketing projects.
              </p>
            </div><!-- / media-body -->
          </div><!-- / media -->
        </div><!-- / .col-md-6 -->
        <div class="col-md-6">
          <div class="media">
            <a class="pull-left" href="#"><span class="dateEl"><em>18</em>Dec</span></a>
            <div class="media-body">
              <h4 class="media-heading">
                <a href="#">Programming 101</a>
              </h4>
              <div class="meta-data">
                <span class="longDate">Dec 18, 2016</span> <span class="timeEl">06:00pm - 08:00pm</span>
              </div>
              <p>
                Take the basic CMS training class to see where things are and how to build custom modules.
              </p>
            </div><!-- / media-body -->
          </div><!-- / media -->
          <div class="media">
            <a class="pull-left" href="#"><span class="dateEl"><em>21</em>Dec</span></a>
            <div class="media-body">
              <h4 class="media-heading">
                <a href="#">Desiging for Mobile</a>
              </h4>
              <div class="meta-data">
                <span class="longDate">Dec 21, 2016</span> <span class="timeEl">10:00am - 12:00pm</span>
              </div>
              <p>
                Get tips and information regarding how to design websites for mobile devices.
              </p>
            </div><!-- / media-body -->
          </div><!-- / media -->
          <div class="media">
            <a class="pull-left" href="#"><span class="dateEl"><em>21</em>Dec</span></a>
            <div class="media-body">
              <h4 class="media-heading">
                <a href="#">Modern Support</a>
              </h4>
              <div class="meta-data">
                <span class="longDate">Dec 22, 2016</span> <span class="timeEl">10:00am - 12:00pm</span>
              </div>
              <p>
                Learn from industry leaders about providing the best support possible.
              </p>
            </div><!-- / media-body -->
          </div><!-- / media -->
        </div><!-- / .col-md-6 -->
      </div><!-- / row -->
      <div class="text-center">
        <br>
        <a class="btn btn-default" href="#">SEE ALL EVENTS</a>
      </div>
    </div>
    <div class="tab-pane fade" id="tab2">
      <div class="row">
        <div class="col-md-6">
          <div class="blogPost--small">
            <div class="media">
              <span class="pull-left"><a href="#"><span class="date"><span>29</span> <small>Nov</small></span></a></span>
              <div class="media-body">
                <h4 class="media-heading">
                  <a href="#">Building In WebCorpCo CMS 8</a>
                </h4>
                <p>
                  Learn about all of the possibilities of web design in our latest CMS release.
                </p>
              </div>
            </div>
          </div><!-- / blogPost -->
          <div class="blogPost--small">
            <div class="media">
              <span class="pull-left"><a href="#"><span class="date"><span>22</span> <small>Nov</small></span></a></span>
              <div class="media-body">
                <h4 class="media-heading">
                  <a href="#">WebCorpCo Named To Inc. 5000</a>
                </h4>
                <p>
                  Inc. magazine today ranked WebCorpCo as the 1,870th fastest growing company on the 34th annual Inc. 5000.
                </p>
              </div>
            </div>
          </div><!-- / blogPost -->
        </div><!-- / .col-md-6 -->
        <div class="col-md-6">
          <div class="blogPost--small">
            <div class="media">
              <span class="pull-left"><a href="#"><span class="date"><span>12</span> <small>Nov</small></span></a></span>
              <div class="media-body">
                <h4 class="media-heading">
                  <a href="#">7 Critical Factors When Choosing A CMS</a>
                </h4>
                <p>
                  Finding a solution that can be tailored to support the needs of your business is more important than ever.
                </p>
              </div>
            </div>
          </div><!-- / blogPost -->
          <div class="blogPost--small">
            <div class="media">
              <span class="pull-left"><a href="#"><span class="date"><span>10</span> <small>Nov</small></span></a></span>
              <div class="media-body">
                <h4 class="media-heading">
                  <a href="#">What Is A Content Management System</a>
                </h4>
                <p>
                  So many acronyms that most of us know a brief amount about, if at all, let alone the meaning of those three little letters we hear so often.
                </p>
              </div>
            </div>
          </div><!-- / blogPost -->
        </div><!-- / row -->
        <div class="text-center">
          <br>
          <a class="btn btn-default" href="#">SEE ALL NEWS</a>
        </div>
      </div>
    </div>
  </div>
              
</div>       
```

## CSS

All required CSS is in news-events-tabs.css


## External Includes

This tutorial contains the following third party resources.

```
<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
<script type="text/javascript" src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
<link rel="stylesheet" type="text/css" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
```
