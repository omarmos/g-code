<template>
    <v-main>
        <div class="space">
            <div class="slider">
                <div class="slider__slide slider__slide--active" data-slide="1">
                    <div class="slider__wrap">
                        <div class="slider__back"></div>
                    </div>
                    <div class="slider__inner">
                        <div class="slider__content">
                            <h1>EXCEL<br>Web and Software Solutions</h1>
                            <h3>“In the information age, build a website before you build a workplace.” – Amit Kalantri</h3>
                            <a class="go-to-next">next</a>
                        </div>
                    </div>
                </div>
                <div class="slider__slide" data-slide="2">
                    <div class="slider__wrap">
                        <div class="slider__back"></div>
                    </div>
                    <div class="slider__inner">
                        <div class="slider__content">
                            <h2>Excel is a Web designing and development company in Sudan which is result oriented. We
                                deliver attractive website designs and execute digital marketing campaigns that lead to the
                                success of the clients</h2><a class="go-to-next">next</a>
                        </div>
                    </div>
                </div>
                <div class="slider__slide" data-slide="3">
                    <div class="slider__wrap">
                        <div class="slider__back"></div>
                    </div>
                    <div class="slider__inner">
                        <div class="slider__content">
                            <h1>Slide <br> Three</h1><a class="go-to-next">next</a>
                        </div>
                    </div>
                </div>
                <div class="slider__indicators"></div>
            </div>
        </div>

    </v-main>
</template>
<script>
import $ from "jquery"

export default {
    name: 'Hero',
    mounted() {
        $(document).ready(function () {
            for (var i = 1; i <= $('.slider__slide').length; i++) {
                $('.slider__indicators').append('<div class="slider__indicator" data-slide="' + i + '"></div>')
            }
            setTimeout(function () {
                $('.slider__wrap').addClass('slider__wrap--hacked');
            }, 1000);
        })

        function goToSlide(number) {
            $('.slider__slide').removeClass('slider__slide--active');
            $('.slider__slide[data-slide=' + number + ']').addClass('slider__slide--active');
        }

        $('.slider__next, .go-to-next').on('click', function () {
            var currentSlide = Number($('.slider__slide--active').data('slide'));
            var totalSlides = $('.slider__slide').length;
            currentSlide++
            if (currentSlide > totalSlides) {
                currentSlide = 1;
            }
            goToSlide(currentSlide);
        })

    },
}
</script>
<style lang="scss">@import '../sass/hero.scss';</style>