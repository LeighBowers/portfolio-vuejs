<template>
  <div class="feat bg-gray pt-5 pb-5">
    <div class="container">
      <div class="row">
        <div class="section-head col-sm-12">
          <h4><span>Port</span>folio</h4>
        </div>
        <div class="col-lg-4 col-sm-6">
          <div class="item">
            <h6>Projects</h6>
            <img
              src="https://i.postimg.cc/DzZTyfg0/IMG-20211029-104425.png"
              class="card-img-top"
              alt="..."
            />

            <p>
              Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean
              commodo ligula eget dolor Aenean massa.
            </p>
          </div>
        </div>
        <div class="col-lg-4 col-sm-6">
          <div class="item">
            <h6>Projects</h6>
            <img
              src="https://i.postimg.cc/QCNVXZHq/IMG-20211029-101053.png"
              class="card-img-top"
              alt="..."
            />
            <p>
              Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean
              commodo ligula eget dolor Aenean massa.
            </p>
          </div>
        </div>
        <div class="col-lg-4 col-sm-6">
          <div class="item">
            <h6>Projects</h6>
            <img
              src="https://i.postimg.cc/QCNVXZHq/IMG-20211029-101053.png"
              class="card-img-top"
              alt="..."
            />
            <p>
              Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean
              commodo ligula eget dolor Aenean massa.
            </p>
          </div>
        </div>
        <div class="col-lg-4 col-sm-6">
          <div class="item">
            <h6>Projects</h6>
            <p>
              Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean
              commodo ligula eget dolor Aenean massa.
            </p>
          </div>
        </div>
        <div class="col-lg-4 col-sm-6">
          <div class="item">
            <h6>Projects</h6>
            <p>
              Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean
              commodo ligula eget dolor Aenean massa.
            </p>
          </div>
        </div>
        <div class="col-lg-4 col-sm-6">
          <div class="item">
            <h6>Projects</h6>
            <p>
              Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean
              commodo ligula eget dolor Aenean massa.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
ul {
  margin: 0;
  padding: 0;
  list-style: none;
}
.card-img-top {
  max-width: 50%;
  height: auto;
}
span,
a,
a:hover {
  display: inline-block;
  text-decoration: none;
  color: inherit;
}
.section-head {
  margin-bottom: 60px;
}

.item {
  background: #fff;
  text-align: center;
  padding: 30px 25px;
  -webkit-box-shadow: 0 0px 25px rgba(0, 0, 0, 0.07);
  box-shadow: 0 0px 25px rgba(0, 0, 0, 0.07);
  border-radius: 20px;
  border: 5px solid rgba(0, 0, 0, 0.07);
  margin-bottom: 30px;
  -webkit-transition: all 0.5s ease 0;
  transition: all 0.5s ease 0;
  transition: all 0.5s ease 0s;
}
.item:hover {
  background: #da680c91;
  box-shadow: 0 8px 20px 0px rgba(0, 0, 0, 0.2);
  -webkit-transition: all 0.5s ease 0;
  transition: all 0.5s ease 0;
  transition: all 0.5s ease 0s;
}

.item:hover h6,
.item:hover p {
  color: rgb(34, 9, 9);
  -webkit-transition: all 0.5s ease 0;
  transition: all 0.5s ease 0;
  transition: all 0.5s ease 0s;
}

.item p {
  font-size: 15px;
  line-height: 26px;
}
.item h6 {
  margin-bottom: 20px;
  color: #2f2f2f;
}
.mission p {
  margin-bottom: 10px;
  font-size: 15px;
  line-height: 28px;
  font-weight: 500;
}

.skills {
  padding-top: 0px;
}
.skills .prog-item {
  margin-bottom: 25px;
}
.skills .prog-item:last-child {
  margin-bottom: 0;
}
.skills .prog-item p {
  font-weight: 500;
  font-size: 15px;
  margin-bottom: 10px;
}
.skills .prog-item .skills-progress {
  width: 100%;
  height: 10px;
  background: #5f0808;
  border-radius: 20px;
  position: relative;
}
</style>