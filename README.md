<ul class="menu">
  <div class="menu_icon"></div>
    <li><a href="#">Home</a></li>
    <li><a href="#">News</a></li>
    <li><a href="#">Contact</a></li>
</ul>
<div class="text">
  <h2>Template with a responsive vertical menu for a blog</h2>
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Est reiciendis repellendus itaque voluptates, omnis nobis suscipit, eaque voluptatum quisquam optio natus facilis nesciunt repudiandae laudantium nostrum nam dolores quae voluptatem.</p>
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Est reiciendis repellendus itaque voluptates, omnis nobis suscipit, eaque voluptatum quisquam optio natus facilis nesciunt repudiandae laudantium nostrum nam dolores quae voluptatem.</p>
  
  <h3>This is the first news !</h3>
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Est reiciendis repellendus itaque voluptates, omnis nobis suscipit, eaque voluptatum quisquam optio natus facilis nesciunt repudiandae laudantium nostrum nam dolores quae voluptatem.</p>
  
  <img src="http://freefunnydogpictures.com/wp-content/uploads/2014/05/picture_1400053660.jpg" />
  
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Est reiciendis repellendus itaque voluptates, omnis nobis suscipit, eaque voluptatum quisquam optio natus facilis nesciunt repudiandae laudantium nostrum nam dolores quae voluptatem.</p>
  
  <h3>This is the second news !</h3>
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Est reiciendis repellendus itaque voluptates, omnis nobis suscipit, eaque voluptatum quisquam optio natus facilis nesciunt repudiandae laudantium nostrum nam dolores quae voluptatem.</p>
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Est reiciendis repellendus itaque voluptates, omnis nobis suscipit, eaque voluptatum quisquam optio natus facilis nesciunt repudiandae laudantium nostrum nam dolores quae voluptatem.</p>
</div>
<style>
  @import url(https://fonts.googleapis.com/css?family=Roboto:400,700);

* {
  padding: 0;
  margin: 0;
}

body {
  background: #ddd;
}


.menu {
  position: fixed;
  display: block;
  width: 130px;
  height: 100%;
  background: #333;
  left: -130px;
  top: 0;
  text-align: center;
  padding-top: 60px;
  -webkit-transition: all .4s ease-in-out ;
  transition: all .4s ease-in-out ;
  &:after {
    position: absolute;
    content: "";
    width: 60px;
    height: 60px;
    background: #333;
    top: 0;
    right: -60px;
    -webkit-transition: all .4s ease-in-out ;
  transition: all .4s ease-in-out ;
  }
  &:hover {
    left: 0;
    &:after {
      right: 0px;
    }
    .menu_icon {
      left:50%;
    }
  }
  li {
    list-style-type: none;
    a {
      color: #FFF;
      text-decoration: none;
      font-family: 'Roboto', sans-serif;
      display: block;
      width: 100%;
      height: 40px;
      line-height: 40px;
      font-size: 18px;
      margin: 10px 0;
      &:hover {
        background: #000;
      }
    }
  }
}

.menu_icon {
  position:absolute;
  top:36px;
  left:158px;
  margin: -10px;
  width:20px;
  height:4px;
  background:#fff;
  z-index:4;
  -webkit-transition: all .4s ease-in-out ;
  transition: all .4s ease-in-out ;
    &:after {
      position:absolute;
      bottom:7px;
      left:0px;
      content:'';
      width:20px;
      height:4px;
      background:#fff;
    }
    &:before {
      position:absolute;
      bottom:-7px;
      left:0px;
      content:'';
      width:20px;
      height:4px;
      background:#fff;
    }
}

.text {
  width: 68%;
  margin: 10px auto 0 auto;
  font-family: 'Roboto', sans-serif;
  color: #333;
  font-size: 18px;
  line-height: 28px;
  margin-top: 10px;
  h2 ,h3 {
    font-size: 30px;
    padding: 20px 0 10px;
    border-bottom: 1px solid #333;
    margin-bottom: 15px;
  }
  h2 {
    font-size: 30px;
    line-height: 42px;
  }
  h3 {
    font-size: 24px;
    line-height: 34px;
  }
  p {
    padding: 10px 0;
  }
  img {
    max-width: 100%;
    height: auto;
    display: block;
    margin: 10px auto;
  }
}

@media only screen and (max-width:1000px) {
  .menu_icon {
    left: 60px;
  }
  .menu {
  position: relative;
  width: 100%;
  height: 60px;
  left: 0px;
  top: 0px;
  padding-top: 0;
  padding-left: 80px;
  &:after {
    display: none;
  }
    &:hover {
      .menu_icon {
          left:60px;
        }
    }
  }
  li {
    float: left;
    margin: 0 20px;
    a {
      padding: 0 10px;
    }
  }
}

  </style>
