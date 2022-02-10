<template>
  <section id="resume">
  <div class="container">
        <h3 class="resume">My Background</h3>
        <div class="row">
            <div class="col-md-12">
                <div class="main-timeline4">
                    <div class="timeline">
                        <span class="timeline-icon"></span>
                        <span class="year">2015</span>
                        <div class="timeline-content">
                            <h3 class="title">Luhlaza High School</h3>
                            <p class="description">
                                A high school that is located in Khayelitsha.
                            </p>
                        </div>
                    </div>
                    <div class="timeline">
                        <span class="timeline-icon"></span>
                        <span class="year">2016</span>
                        <div class="timeline-content">
                            <h3 class="title">pascap trust</h3>
                            <p class="description">
                                An after school programme that helps children with their school work.
                            </p>
                        </div>
                    </div>
                    <div class="timeline">
                        <span class="timeline-icon"></span>
                        <span class="year">2017</span>
                        <div class="timeline-content">
                            <h3 class="title">rise young women's club</h3>
                            <p class="description">
                                A club that creates a safe space for women.
                            </p>
                        </div>
                    </div>
                    <div class="timeline">
                        <span class="timeline-icon"></span>
                        <span class="year">2019</span>
                        <div class="timeline-content">
                            <h3 class="title">ikamva youth</h3>
                            <p class="description">
                               A tutoring programme for children in disadvantaged places.
                            </p>
                        </div>
                    </div>
                     <div class="timeline">
                        <span class="timeline-icon"></span>
                        <span class="year">2021</span>
                        <div class="timeline-content">
                            <h3 class="title">lifechoices coding academy</h3>
                            <p class="description">
                               A coding academy in lansdowne
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
 </section>
</template>
<script>

export default {
  name: 'Resume',
  components: {
  }
}
</script>

<style scoped>
.resume{
    font-family: sans-serif;
    font-size: 3rem;
    font-weight: 700;
    color: #ea4343;
    letter-spacing: -.2px;
    display: inline-block;
    margin-bottom: 6px;
    padding-bottom:15px;
}
.main-timeline4 {
    overflow: hidden;
    position: relative
}

.main-timeline4:after,
.main-timeline4:before {
    content: "";
    display: block;
    width: 100%;
    clear: both
}

.main-timeline4:before {
    content: "";
    width: 3px;
    height: 100%;
    background: #d6d5d5;
    position: absolute;
    top: 30px;
    left: 50%
}

.main-timeline4 .timeline {
    width: 50%;
    float: left;
    padding-right: 30px;
    position: relative
}

.main-timeline4 .timeline-icon {
    width: 32px;
    height: 32px;
    border-radius: 50%;
    background: #fff;
    border: 3px solid #ea4343;
    position: absolute;
    top: 5.5%;
    right: -17.5px
}

.main-timeline4 .year {
    display: block;
    padding: 10px;
    margin: 0;
    font-size: 30px;
    color: #fff;
    border-radius: 0 50px 50px 0;
    background: #ea4343 ;
    text-align: center;
    position: relative
}

.main-timeline4 .year:before {
    content: "";
    border-top: 35px solid #ea4343 ;
    border-left: 35px solid transparent;
    position: absolute;
    bottom: -35px;
    left: 0
}

.main-timeline4 .timeline-content {
    padding: 30px 20px;
    margin: 0 45px 0 35px;
    background: #f2f2f2
}

.main-timeline4 .title {
    font-size: 19px;
    font-weight: 700;
    color: #504f54;
    margin: 0 0 10px
}

.main-timeline4 .description {
    font-size: 14px;
    color: #7d7b7b;
    margin: 0
}

.main-timeline4 .timeline:nth-child(2n) {
    padding: 0 0 0 30px
}

.main-timeline4 .timeline:nth-child(2n) .timeline-icon {
    right: auto;
    left: -14.5px
}

.main-timeline4 .timeline:nth-child(2n) .year {
    border-radius: 50px 0 0 50px;
    background: #7d7d7d
}

.main-timeline4 .timeline:nth-child(2n) .year:before {
    border-left: none;
    border-right: 35px solid transparent;
    left: auto;
    right: 0
}

.main-timeline4 .timeline:nth-child(2n) .timeline-content {
    text-align: right;
    margin: 0 35px 0 45px
}

.main-timeline4 .timeline:nth-child(2) {
    margin-top: 170px
}

.main-timeline4 .timeline:nth-child(odd) {
    margin: -175px 0 0
}

.main-timeline4 .timeline:nth-child(even) {
    margin-bottom: 80px
}

.main-timeline4 .timeline:first-child,
.main-timeline4 .timeline:last-child:nth-child(even) {
    margin: 0
}

.main-timeline4 .timeline:nth-child(2n) .timeline-icon {
    border-color: #7d7d7d
}

.main-timeline4 .timeline:nth-child(2n) .year:before {
    border-top-color: #7d7d7d
}

.main-timeline4 .timeline:nth-child(3n) .timeline-icon {
    border-color: #ea4343
}

.main-timeline4 .timeline:nth-child(3n) .year {
    background: #ea4343
}

.main-timeline4 .timeline:nth-child(3n) .year:before {
    border-top-color: #ea4343
}

.main-timeline4 .timeline:nth-child(4n) .timeline-icon {
    border-color: #7d7d7d
}

.main-timeline4 .timeline:nth-child(4n) .year {
    background: #7d7d7d
}

.main-timeline4 .timeline:nth-child(4n) .year:before {
    border-top-color: #7d7d7d
}

@media only screen and (max-width:767px) {
    .main-timeline4 {
        overflow: visible
    }
    .main-timeline4:before {
        top: 0;
        left: 0
    }
    .main-timeline4 .timeline:nth-child(2),
    .main-timeline4 .timeline:nth-child(even),
    .main-timeline4 .timeline:nth-child(odd) {
        margin: 0
    }
    .main-timeline4 .timeline {
        width: 100%;
        float: none;
        padding: 0 0 0 30px;
        margin-bottom: 20px!important
    }
    .main-timeline4 .timeline:last-child {
        margin: 0!important
    }
    .main-timeline4 .timeline-icon {
        right: auto;
        left: -14.5px
    }
    .main-timeline4 .year {
        border-radius: 50px 0 0 50px
    }
    .main-timeline4 .year:before {
        border-left: none;
        border-right: 35px solid transparent;
        left: auto;
        right: 0
    }
    .main-timeline4 .timeline-content {
        margin: 0 35px 0 45px
    }
}

</style>